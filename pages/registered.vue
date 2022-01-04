<template>
  <div class="submit">
    <div class="submit-content">
      <img src="@/assets/images/Partnership-bro-1.png" alt="" />
      <h1>Thank you for registering!</h1>
      <p>Check your email for the code for the 6 months free filing</p>
    </div>
  </div>
</template>

<script>
export default {
};
</script>

<style lang="scss" scoped>
.submit {
  background: #ff6600;
  margin-bottom: 60px;
  padding: 40px;
  width: auto;

  .submit-content {
    background: #ffffff;
    width: 70%;
    margin: 0 auto;
    padding: 14px 150px;
    border-radius: 15px;

    @media (max-width: 376px){
      width: 100%;
      padding: 14px 20px;
      margin: 14px auto;
    }

    img {
      position: relative;
      width: 100%;
    }

    h1 {
      font-family: Roboto;
      font-style: normal;
      font-weight: bold;
      font-size: 24px;
      line-height: 28px;
      text-align: center;
      margin-bottom: 20px;
    }

    p {
      font-family: Roboto;
      font-style: normal;
      font-weight: 300;
      font-size: 14px;
      line-height: 16px;
      text-align: center;
    }
  }
}
</style>
