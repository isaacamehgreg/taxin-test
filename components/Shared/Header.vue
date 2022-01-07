<template>
  <div class="header d-sm-flex align-center justify-sm-center justify-md-space-between mx-12">
    <NuxtLink to="/"><img src="@/assets/images/logo.png" class="social-icon" alt=""></NuxtLink>
    <div class="socials d-flex align-center">
      <NuxtLink to="/" class="join-us me-4">Join us</NuxtLink>
      <NuxtLink to="/"><img src="@/assets/images/Facebook.png" class="social-icon me-3" alt=""></NuxtLink>
      <NuxtLink to="/"><img src="@/assets/images/LinkedIN.png" class="social-icon me-3" alt=""></NuxtLink>
      <NuxtLink to="/"><img src="@/assets/images/Twitter.png" class="social-icon me-3" alt=""></NuxtLink>
      <NuxtLink to="/"><img src="@/assets/images/Instagram.png" class="social-icon" alt=""></NuxtLink>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
  img {
    width: 200px;
  }
  .socials {
    .join-us {
      text-decoration: none;
      color: #7C7A7A;
      font-size: 20px;
      font-weight: 600;
      margin-top: -5px;
    }
    .social-icon {
      padding-bottom: 0;
    }
    img {
      width: 35px;
    }
  }

  .header {
    margin-right: 0 !important;
    margin-left: 0 !important;
  }
</style>