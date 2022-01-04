<template>
  <div>
    <StepperForm />
  </div>
</template>

<script>
  import StepperForm from "@/components/CompanyRegistration/StepperForm.vue"
  export default {
    layout: 'welcomeBack',
    components: {
      'StepperForm': StepperForm
    }
  }
</script>

<style lang="scss" scoped>

</style>