<template>
  <v-form ref="form" lazy-validation class="form">
    <p class="form-title mt-3">Please verify your information</p>

    <div class="info-container d-md-flex justify-space-between">
      <div>
        <div class="d-flex align-center form-title">
          <p class="">Personal Information</p>
          <v-icon class="mb-3 ms-2 orange--text">{{ icons.mdiPencil }}</v-icon>
        </div>
        <p class="">Full Name: <b>Mai</b></p>
        <p class="">Title: <b>Tax Advisor</b></p>
        <p class="">Email: <b>mystars70@mail.com</b></p>
        <p class="">Telephone: <b>5039169018</b></p>
      </div>

      <div>
        <div class="d-flex align-center form-title">
          <p class="">Company Information</p>
          <v-icon class="mb-3 ms-2 orange--text">{{ icons.mdiPencil }}</v-icon>
        </div>
        <p class="">Company Name: <b>ABC Tax LLC</b></p>
        <p class="">Address: <b>12345 Dana Street</b></p>
        <p class="">City: <b>Houstan</b></p>
        <p class="">State: <b>TX</b></p>
        <p class="">Postal Code: <b>77854</b></p>
        <p class="">Country: <b>USA</b></p>
      </div>
    </div>
  </v-form>
</template>

<script>
import { mdiPencil } from "@mdi/js";

export default {
  data: () => ({
    icons: {
      mdiPencil,
    },
  }),
};
</script>

<style lang="scss" scoped>
.form {
  padding: 15px 50px;

  @media (max-width: 376px){
    padding: 7px 15px;
  }

  .form-title {
    font-family: Roboto;
    font-style: normal;
    font-weight: bold;
    font-size: 22px;
    line-height: 25px;
    text-align: center;
    color: rgba(0, 0, 0, 0.68);
    margin-top: 45px;
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
