<template>
  <v-app>
    <v-main>
      <v-container>
        <Header />
        <Nuxt />
      </v-container>
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "@/components/Shared/Header.vue"
import Footer from "@/components/Shared/Footer.vue"
export default {
  name: 'DefaultLayout',
  components: {
    'Header': Header,
    'Footer': Footer
  },
  data () {
    return {
    }
  }
}
</script>
