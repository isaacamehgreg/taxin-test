<template>
  <v-app>
    <v-main>
      <Header />
      <WelcomeBackHeader />
      <v-container><Nuxt /></v-container>
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "@/components/Shared/Header.vue"
import Footer from "@/components/Shared/Footer.vue"
import WelcomeBackHeader from "@/components/Shared/WelcomeBackHeader.vue"
export default {
  name: 'DefaultLayout',
  components: {
    'Header': Header,
    'Footer': Footer,
    'WelcomeBackHeader': WelcomeBackHeader
  },
  data () {
    return {
    }
  }
}
</script>
