<template>
  <div>
    <Hero />
    <Banner />
    <Faq />
  </div>
</template>

<script>
import Hero from "@/components/HomePage/Hero.vue"
import Banner from "@/components/HomePage/Banner.vue"
import Faq from "@/components/HomePage/Faq.vue"
export default {
  name: 'IndexPage',
  components: {
    'Hero': Hero,
    'Banner': Banner,
    'Faq': Faq
  },
}
</script>
