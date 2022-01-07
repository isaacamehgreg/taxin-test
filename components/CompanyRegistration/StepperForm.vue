<template>
  <v-stepper v-model="step" alt-labels flat>
    <v-stepper-header>
      <v-stepper-step step="1" :complete="step > 1">Register</v-stepper-step>
      <v-divider :class="[{'complete' : step > 1}]"></v-divider>
      <v-stepper-step step="2" :complete="step > 2">Verify</v-stepper-step>
      <v-divider :class="[{'complete' : step > 2}]"></v-divider>
      <v-stepper-step step="3" :complete="step > 3">Tax Report Bank</v-stepper-step>
    </v-stepper-header>

    <v-stepper-items>
      <v-stepper-content step="1">
        <v-card elevation="0" class="mb-12 rounded-xl" color="#F4F4F4">
          <FormPage1 />
        </v-card>
        <div class="d-flex justify-center">
          <v-btn class="custom-btn" color="success" @click="++step"> Proceed </v-btn>
        </div>
      </v-stepper-content>

      <v-stepper-content step="2">
        <v-card elevation="0" class="mb-12 rounded-xl" color="#F4F4F4">
          <FormPage2 />
        </v-card>

        <div class="d-flex justify-center">
          <v-btn class="custom-btn" outlined @click="--step"> Back </v-btn>
          <v-btn class="custom-btn ml-3" color="success" @click="++step"> Continue </v-btn>
        </div>

      </v-stepper-content>

      <v-stepper-content step="3">
        <v-card elevation="0" class="mb-12 rounded-xl" color="#F4F4F4">
          <FormPage3 />
        </v-card>

        <div class="d-flex justify-center">
          <v-btn class="custom-btn" outlined @click="--step"> Back </v-btn>
          <v-btn class="custom-btn ml-3" color="success" @click="++step"> Continue </v-btn>
        </div>
      </v-stepper-content>

      <v-stepper-content step="4">
        <v-card elevation="0" class="mb-12 rounded-xl" color="#F4F4F4">
          <FormPage4 />
        </v-card>
      </v-stepper-content>
    </v-stepper-items>
  </v-stepper>
</template>

<script>
import FormPage1 from "@/components/CompanyRegistration/FormPage1.vue"
import FormPage2 from "@/components/CompanyRegistration/FormPage2.vue"
import FormPage3 from "@/components/CompanyRegistration/FormPage3.vue"
import FormPage4 from "@/components/CompanyRegistration/FormPage4.vue"
export default {
  data() {
    return {
      step: 1
    };
  },
  components: {
    'FormPage1': FormPage1,
    'FormPage2': FormPage2,
    'FormPage3': FormPage3,
    'FormPage4': FormPage4,
  }
};
</script>

<style lang="sass" scoped>
</style>
