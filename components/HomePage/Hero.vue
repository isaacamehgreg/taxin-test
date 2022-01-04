<template>
  <div class="hero-container d-md-flex justify-space-between">
    <img src="@/assets/images/hero_img_1.png" class="hero-img-1" alt="" />
    <Form />
    <img src="@/assets/images/hero_img_2.png" class="hero-img-2" alt="" />
  </div>
</template>

<script>
import Form from "@/components/HomePage/Form.vue";
export default {
  components: {
    Form: Form,
  },
};
</script>

<style lang="scss" scoped>

.hero-container {
  // display: flex;
  // justify-content: space-between;
  gap: 11px;
  margin-bottom: 19px;

  .hero-img-1,
  .hero-img-2 {
    height: 470px;
    @media (max-width: 768px){
      height: 350px;
    }
    @media (max-width: 376px){
      width: 100%;
    }
  }

  .hero-img-2 {
    @media (max-width: 376px){
      display: none;
    }
  }
}

</style>