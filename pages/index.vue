<template>
  <div class="home">
    <div class="bg-hero" :style="{ backgroundImage: `url(${backgroundUrl})` }">

    </div>
    <div class="h-screen">

    </div>
  </div>
</template>

<script>
import backgroundUrl from '~/assets/img/wave.svg'
export default {
  name: 'IndexPage',
  data() {
    return {
      backgroundUrl
    }
  },
  head() {
      return {
        title: "Satrio Nugroho",
        meta: [
          // hid is used as unique identifier. Do not use `vmid` for it as it will not work
          {
            hid: 'My Portofolio',
            name: 'My Portofolio',
            content: 'My Portofolio'
          }
        ]
      }
    }
}
</script>
<style scoped>
.bg-hero {
  background-position: center center;
  background-repeat:  no-repeat;
  background-size: cover;
  height: 100vh;
}
</style>
