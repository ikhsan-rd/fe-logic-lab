<script setup>
import { ref } from "vue";
const heroImage = ref(
  "my-vue-app/src/assets/hero-section/hero-section (resize).png"
);

// const isMobileMenuOpen = ref(false);

// const toggleMenu = () => {
//   isMobileMenuOpen.value = !isMobileMenuOpen.value;
// };
</script>
<template>
  <section id="aboutUs" class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
    <div class="sm:mb-3 sm:flex sm:justify-center">
      <div class="text-center">
        <h1 class="title capitalize text-orange-500">Tentang Logic Lab</h1>
        <p class="subtitle font-semibold text-gray-500">
          Saat ini, kami berfokus pada dua bagian utama, yaitu :
        </p>
      </div>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      <div class="block max-w-sm p-6 rounded-md hover:bg-gray-100">
        <img
          src="../assets/about-us/left-hand.png"
          class="items-center"
          alt="image"
        />
        <h3 class="mb-2 text-2xl font-bold text-gray-900 capitalize">
          layanan professional
        </h3>
      </div>
      <div class="block max-w-sm p-6 rounded-md hover:bg-gray-100">
        <img
          src="../assets/about-us/right-hand.png"
          class="items-center"
          alt="image"
        />
        <h3 class="mb-2 text-2xl font-bold text-gray-900 capitalize">
          komunitas belajar
        </h3>
      </div>
    </div>
  </section>
</template>
<style scoped>
@import url(../../tailwindcss/input.css);
@import url(../../tailwindcss/output.css);
</style>
