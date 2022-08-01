<template>
  <div class="h-screen justify-center items-center flex ">
    <h1 v-if="error.statusCode === 404" class="my-auto">Page not found</h1>
  </div>
</template>

<script>
export default {
  name: 'ErrorMy',
  layout: 'error',
  props: ['myError'],
}
</script>

<style>

</style>
