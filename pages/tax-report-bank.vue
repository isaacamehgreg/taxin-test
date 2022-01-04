<template>
  <div class="tax-report-bank">
    <img src="@/assets/images/Illustration2.png" class="img" alt="" />
    <p class="text">
      As we take the AI journey to tax technology, we are missing tax data to
      build a <br />
      smart tax engine. With this in mind, we are reaching out to Tax Advisors
      to build <br />
      the missing reports with MFExcise Cloud Technology and take advantage of
      <br />
      filing 12 months for free.
    </p>

    <!-- FORM -->
    <div class="form">
      <p class="form-title">
        File 12 months free for each report that you help build.
      </p>
      <p class="text">
        File 12 months free for each report that you help build.
      </p>
      <div class="d-md-flex justify-space-between">
        <v-text-field
          v-model="firstName"
          label="File Name"
          required
          dense
          hide-details="hide"
          outlined
          class="form-text-field mb-3"
        ></v-text-field>
        <v-text-field
          v-model="firstName"
          label="State"
          required
          dense
          hide-details="hide"
          outlined
          class="form-text-field mb-3"
        ></v-text-field>
      </div>
    </div>
    <v-btn
      color="#22C855"
      class="submit-button white--text"
      @click="resetValidation"
    >
      Submit
    </v-btn>
  </div>
</template>

<script>
export default {
  layout: "welcomeBack",
};
</script>

<style lang="scss" scoped>
.tax-report-bank {
  text-align: center;

  .img {
    width: 50%;
    margin-top: 24px;
    margin-bottom: 39px;

    @media (max-width: 376px) {
      width: 100%;
    }
  }

  .text {
    font-family: Roboto;
    font-style: normal;
    font-weight: 300;
    font-size: 22px;
    line-height: 30px;
    color: #000000;
    margin-bottom: 40px;
  }

  .form {
    background: #f4f4f4;
    padding: 20px 40px 36px;
    border-radius: 15px;

    @media (max-width: 376px) {
    padding: 40px 40px 40px;
    }

    .form-title {
      font-family: Roboto;
      font-style: normal;
      font-weight: bold;
      font-size: 24px;
      line-height: 16px;
      text-align: center;
      color: #000000;
      margin-bottom: 13px;

      @media (max-width: 376px) {
        line-height: 25px;
      }
    }

    .text {
      margin-bottom: 47px;
    }

    div {
      gap: 25px;
    }
  }

  .submit-button {
    margin: 25px 0 45px;
    padding: 10px 30px;
  }
}
</style>
