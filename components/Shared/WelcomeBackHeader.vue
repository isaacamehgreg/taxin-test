<template>
  <div class="header">
    <h1>Welcome back, Mai!</h1>
    <v-text-field
      v-model="code"
      placeholder="Enter Your Code"
      required
      dense
      hide-details="hide"
      outlined
      class="code-input"
    ></v-text-field>
  </div>
</template>

<script>
export default {
  data: () => ({
    code: "",
  }),
};
</script>

<style lang="scss" scoped>
.header {
  background: #22c855;
  padding: 25px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 20px;

  h1 {
    font-family: Roboto;
    font-style: normal;
    font-weight: bold;
    // font-size: 24px;
    line-height: 28px;
    text-align: center;
    color: #ffffff;
  }

  ::v-deep .code-input {
    fieldset {
      text-align: center;
      border: 1px solid #d8d8d8;
      border-radius: 10px;
      background: #ffffff;
    }
  }

  .code-input {
    margin: 0 auto; 
  }
}
</style>
