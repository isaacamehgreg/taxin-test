<template>
  <v-form ref="form" v-model="valid" lazy-validation class="form">
    <p class="form-title mt-3">Get Started</p>
    <p class="text">
      File free for six months on reports stored in our <br>
      <NuxtLink to="/" class="link">Tax Report Bank</NuxtLink>
    </p>
    <div class="d-flex justify-space-between">
      <v-text-field
        v-model="firstName"
        label="First Name"
        required
        dense
        hide-details="hide"
        outlined
        class="form-text-field me-3 mb-3"
      ></v-text-field>

      <v-text-field
        v-model="lastName"
        label="Last Name"
        required
        dense
        hide-details="hide"
        outlined
        class="form-text-field"
      ></v-text-field>
    </div>

    <v-text-field
      v-model="title"
      label="Title"
      required
      dense
      hide-details="hide"
      outlined
      class="form-text-field mb-3"
    ></v-text-field>

    <v-text-field
      v-model="email"
      label="Email"
      required
      dense
      hide-details="hide"
      outlined
      class="form-text-field mb-3"
    ></v-text-field>

    <v-text-field
      v-model="phone"
      label="Phone"
      required
      dense
      hide-details="hide"
      outlined
      class="form-text-field mb-6"
    ></v-text-field>

    <v-btn
      color="#FF6600"
      class="submit-button white--text"
      @click="resetValidation"
    >
      Submit
    </v-btn>
  </v-form>
</template>

<script>
export default {
  data: () => ({
    firstName: "",
    lastName: "",
    title: "",
    email: "",
    phone: "",
  }),

  methods: {
    validate() {
      this.$refs.form.validate();
    },
    reset() {
      this.$refs.form.reset();
    },
    resetValidation() {
      this.$refs.form.resetValidation();
    },
  },
};
</script>

<style lang="scss" scoped>
.form {
  background: #f6f6f6;
  padding: 20px;
  box-shadow: 2px 2px 20px 2px rgba(0, 0, 0, 0.25);
  border-radius: 10px;

  .form-title {
    font-family: Poppins;
    font-style: normal;
    font-weight: 600;
    font-size: 30px;
    color: #ff6600;
    line-height: 27px;
    text-align: center;
  }

  .submit-button {
    font-family: Roboto;
    font-weight: 700;
    border-radius: 10px;
    width: 100%;
    padding: 20px;
  }
  ::v-deep .form-text-field {
    fieldset {
      border: 1px solid #d8d8d8;
      border-radius: 10px;
      background: #ffffff;
    }
  }
}
</style>
