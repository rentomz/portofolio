<template>
  <div class="home">
    <div
      class="bg-hero"
      :style="{ backgroundImage: `url(${backgroundUrl})` }"
    ></div>
    <div>
      <ins
        class="adsbygoogle"
        style="display: block"
        data-ad-client="ca-pub-3859502428144967"
        data-ad-slot="7858255558"
        data-ad-format="auto"
        data-full-width-responsive="true"
      ></ins>
    </div>
    <div class="h-screen"></div>
  </div>
</template>

<script>
import backgroundUrl from '~/assets/img/wave.svg'
export default {
  name: 'IndexPage',
  data() {
    return {
      backgroundUrl,
    }
  },
  head() {
    return {
      title: 'Satrio Nugroho',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'My Portofolio',
          name: 'My Portofolio',
          content: 'My Portofolio',
        },
      ],
    }
  },
}
</script>
<style scoped>
.bg-hero {
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}
</style>
