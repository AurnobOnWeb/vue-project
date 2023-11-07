<template>
  <Header />
  <div class="w-full h-auto bg-gray-100 text-black lg:flex lg:justify-center">
    <div class="lg:w-[80%] xl:w-[70%] lg:mx-0">
      <router-view></router-view>
    </div>
  </div>
  <Footer />
</template>

<script setup>
import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";
</script>

<style lang="scss" scoped></style>
