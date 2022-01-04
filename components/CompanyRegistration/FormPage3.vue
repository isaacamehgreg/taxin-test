<template>
  <v-form ref="form" v-model="valid" lazy-validation class="form">
    <div class="d-md-flex text-center justify-center">
      <p class="form-title mt-3 me-3">
        Select one report to file free for 6 months!
      </p>
      <NuxtLink to="/" class="link form-title mt-3"
        >Don’t see the report you need?</NuxtLink
      >
    </div>

    <v-expansion-panels accordion>
      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>IRS ExSTARS</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel
        class="expansion-item mb-3 rounded-xl font-weight-bold"
      >
        <v-expansion-panel-header>Alabama</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Arkansas</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Georgia</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Illinois</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Indiana</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Kentucky</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Massachusetts</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Minnesota</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Missouri</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>

      <v-expansion-panel class="mb-3 rounded-xl font-weight-bold">
        <v-expansion-panel-header>Nebraska</v-expansion-panel-header>
        <v-expansion-panel-content>
          <v-checkbox
            v-model="checkbox1"
            :label="`MFT-TOM Terminal Operator`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox2"
            :label="`MFT-SDR Supplier/Distribution/Blender`"
          ></v-checkbox>
          <v-checkbox
            v-model="checkbox3"
            :label="`MFT-CCR Carrier`"
          ></v-checkbox>
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </v-form>
</template>

<script>
export default {
  data() {
    return {
      checkbox1: false,
      checkbox2: false,
      checkbox3: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.form {
  padding: 15px 50px;

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

  v-expansion-panel {
    border-top: 0;
  }

}
.v-expansion-panel:not(:first-child) {
  &::after {
    border-top: none;
  }
}
</style>
