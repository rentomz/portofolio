<template>
  <!-- navbar goes here -->
  <nav class="bg-white shadow-md">
    <div class="max-w-7xl mx-auto px-6">
      <div class="flex justify-between">
        <div class="flex space-x-4">
          <!-- logo -->
          <div>
            <nuxt-link
              to="/"
              class="flex items-center py-5 px-2"
            >
              <!-- <svg
                class="h-6 w-6 mr-1 text-blue-400"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"
                />
              </svg> -->
              <p class="font-bold f-head text-2xl">SAI<span class="c-blue">ROZ.</span></p>
            </nuxt-link>
          </div>

          <!-- primary nav -->
          <!-- <div class="hidden md:flex items-center space-x-1">

          </div> -->
        </div>

        <!-- secondary nav -->
        <div class="hidden md:flex items-center text-lg space-x-1">
          <nuxt-link to="/" class="py-5 px-6 hover:text-blue-400"
              >Home</nuxt-link
            >
          <nuxt-link to="/project" class="py-5 px-6 hover:text-blue-400"
              >Project</nuxt-link
            >
            <nuxt-link to="#" class="py-5 px-6 hover:text-blue-400"
              >Contact</nuxt-link
            >
        </div>

        <!-- mobile button goes here -->
        <div class="md:hidden flex items-center">
          <button class="mobile-menu-button" @click="hidden = !hidden">
            <svg
              class="w-6 h-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>

    <!-- mobile menu -->
    <div  v-if="hidden" :class="'mobile-menu md:hidden'">
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-200">Home</a>
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-200">Project</a>
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-200">Contact</a>
    </div>
  </nav>
</template>

<script>
export default {
  name: "ComponentHeader",
  data() {
    return {
      hidden: true,
    }
  },
}
</script>

<style></style>
