<template>
  <v-app dark>
    <!-- Header -->
    <Header />

    <v-main>
        <nuxt />
    </v-main>

    <!-- Footer -->
    <Footer />
  </v-app>
</template>

<script>
import Header from '~/components/default/Header.vue'
import Footer from '~/components/default/Footer.vue'
export default {
  components: {
    Header,
    Footer
  }
}
</script>
