<template>
  <v-form ref="form" lazy-validation class="form">
    <p class="form-title mt-3">Company Information</p>

    <v-text-field
      v-model="companyName"
      label="Company Name"
      required
      dense
      hide-details="hide"
      outlined
      class="form-text-field mb-3"
    ></v-text-field>

    <v-text-field
      v-model="address"
      label="Address"
      required
      dense
      hide-details="hide"
      outlined
      class="form-text-field mb-3"
    ></v-text-field>

    <div class="d-flex justify-space-between">
      <v-text-field
        v-model="city"
        label="City"
        required
        dense
        hide-details="hide"
        outlined
        class="form-text-field me-3 mb-3"
      ></v-text-field>

      <v-text-field
        v-model="state"
        label="State"
        required
        dense
        hide-details="hide"
        outlined
        class="form-text-field"
      ></v-text-field>
    </div>

    <div class="d-flex justify-space-between">
      <v-text-field
        v-model="postalCode"
        label="Postal Code"
        required
        dense
        hide-details="hide"
        outlined
        class="form-text-field me-3 mb-3"
      ></v-text-field>

      <v-text-field
        v-model="county"
        label="Last Name"
        required
        dense
        hide-details="hide"
        outlined
        class="form-text-field"
      ></v-text-field>
    </div>
  </v-form>
</template>

<script>
export default {
  data() {
    return {
      companyName: "",
      address: "",
      city: "",
      state: "",
      postalCode: "",
      county: "",
    };
  },
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
    line-height: 16px;
    text-align: center;
    color: rgba(0, 0, 0, 0.68);
    margin-bottom: 45px;
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
