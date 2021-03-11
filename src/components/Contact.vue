<template>
  <section class="contact-section bg-grey-1">
    <q-form @submit="submitContactForm()">
      <div class="row">
        <q-space />
        <div class="col-lg-7 col-md-8 col-sm-12 q-px-lg">
          <div class="row q-px-md q-pt-xl">
            <div class="text-h4 blueballoon-font weight-600 text-grey-9">
              Escribenos:
            </div>
          </div>
          <div class="row">
            <div class="col-lg-6 col-md-6 col-sm-6 col-xs-12 q-pa-md">
              <q-input
                label="Nombre"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
                v-model="formFields.name"
              />
            </div>
            <div class="col-lg-6 col-md-6 col-sm-6 col-xs-12 q-pa-md">
              <q-input
                label="Telefono"
                type="number"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
                v-model="formFields.phone"
              />
            </div>
          </div>
          <div class="row">
            <div class="col q-pa-md">
              <q-input
                label="Correo"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
                v-model="formFields.email"
              />
            </div>
          </div>
          <div class="row">
            <div class="col q-pa-md">
              <q-input
                label="Mensaje"
                type="textarea"
                rows="7"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
                v-model="formFields.message"
              />
            </div>
          </div>
          <div class="row q-px-md">
            <q-space />
            <q-btn
              rounded
              class="blueballoon-font text-bold gradient-two text-white"
              label="Enviar"
              no-caps
              type="submit"
              :loading="isLoading"
            />
          </div>
        </div>
        <q-space />
      </div>
    </q-form>
    <q-dialog v-model="dialog">
      <q-card flat style="border-radius: 25px">
        <q-card-section class="text-center">
          <i
            class="fas fa-check fa-4x text-primary"
            v-if="dialogContent.success"
          ></i>
          <i class="fas fa-exclamation fa-4x text-red-7" v-else></i>
        </q-card-section>
        <q-card-section class="blueballoon-font text-center">
          <div class="text-h6 w700">{{ dialogContent.message }}</div>
        </q-card-section>
        <q-card-actions>
          <q-space />
          <q-btn
            label="Aceptar"
            v-close-popup
            flat
            rounded
            color="dark"
            class="blueballoon-font text-bold"
          />
        </q-card-actions>
      </q-card>
    </q-dialog>
  </section>
</template>

<script>
import emailjs from "emailjs-com";

export default {
  data() {
    return {
      isLoading: false,
      formFields: {
        name: "",
        phone: "",
        email: "",
        message: "",
      },
      validEmail: /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/,
      dialog: false,
      dialogContent: {
        success: false,
        message: "",
      },
    };
  },
  methods: {
    submitContactForm() {
      this.isLoading = true;
      if (!this.validateForm()) {
        this.setDialogContent(
          false,
          "Debes llenar todos los campos para enviar el mensaje."
        );
        this.dialog = true;
        this.isLoading = false;
        return;
      } else if (!this.validateEmail()) {
        this.setDialogContent(
          false,
          "Debes ingresar un correo valido para poder contactarte."
        );
        this.dialog = true;
        this.isLoading = false;
        return;
      } else {
        emailjs
          .send(
            "gmail",
            "template_zgghba3",
            this.formFields,
            "user_l9KYZVj8DNvwXi3kegar5"
          )
          .then(
            (result) => {
              console.log(result);
              this.setDialogContent(true, "Mensaje enviado con exito.");
              this.dialog = true;
              this.isLoading = false;
              this.clearForm();
            },
            (error) => {
              this.setDialogContent(
                false,
                "Le sentimos hubo un error puedes intentarlo mas tarde plzzzzzz"
              );
              this.dialog = true;
              this.isLoading = false;
              console.log(error);
            }
          );
      }
    },
    clearForm() {
      this.formFields = {
        name: "",
        phone: "",
        email: "",
        message: "",
      };
    },
    validateForm() {
      if (
        !this.formFields.name.replace(/\s/g, "") ||
        !this.formFields.phone.replace(/\s/g, "") ||
        !this.formFields.email.replace(/\s/g, "") ||
        !this.formFields.message.replace(/\s/g, "")
      )
        return false;
      else return true;
    },
    validateEmail() {
      return this.validEmail.test(this.formFields.email);
    },
    setDialogContent(success, message) {
      this.dialogContent.success = success;
      this.dialogContent.message = message;
    },
  },
};
</script>
