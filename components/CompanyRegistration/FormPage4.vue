<template>
  <div class="main-container">
    <p class="text font-weight-bold">Congratulations!</p>
    <div class="text-container">
      <p class="text">
        You are confirmed to file Report Name <br />
        free for the next 6 months. <br />
        Check your email for details to start filing!
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
    };
  },
};
</script>

<style lang="scss" scoped>
.main-container {
  padding: 30px;
  border-radius: 15px;

  .text-container {
    background: #ffffff;
    padding: 30px;
    border-radius: 15px;

    .text {
      color: rgba(0, 0, 0, 0.68);
    }
  }
}
</style>
