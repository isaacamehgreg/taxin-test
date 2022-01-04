<template>
  <div class="submit-conainer">
    <img src="@/assets/images/Illustration1.png" class="img" alt="" />
    <div class="thank-you-card">
      <p class="thank-you-card-title">Thank You!</p>
      <div>
        <p class="text">
          We are so excited to start this AI Tax journey with you.
        </p>
        <p class="text">Check your email for details to get started.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "welcomeBack",
};
</script>

<style lang="scss" scoped>
.submit-conainer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 50px;
  margin: 55px 0 85px;

  @media (max-width: 376px) {
    flex-direction: column;
    gap: 0px;
  }

  .img {
    width: 50%;

    @media (max-width: 376px) {
      width: 100%;
      flex-direction: column;
    }
  }

  .thank-you-card {
    text-align: center;
    background: #ff6600;
    border-radius: 15px;
    padding: 30px 45px;

    .thank-you-card-title {
      font-family: Poppins;
      font-style: normal;
      font-weight: 600;
      font-size: 30px;
      color: #ffffff;
      line-height: 27px;
      text-align: center;
      margin-bottom: 25px;
    }

    div {
      background: #ffffff;
      border-radius: 15px;
      padding: 35px 65px;

      @media (max-width: 376px) {
        padding: 35px 35px;
      }

      .text {
        font-family: Roboto;
        font-style: normal;
        font-weight: 300;
        font-size: 22px;
        line-height: 30px;
        color: #000000;
      }
    }
  }
}
</style>
