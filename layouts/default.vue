<template>
  <div>
    <Header />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'
export default {
  name: 'DefaultName',
  components: { Header, Footer },
}
</script>

<style>
body {
  color: #001427;
  font-family: 'Inter', sans-serif;
}
</style>
