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
  <!-- Hero section / home -->
  <main
    id="home"
    class="section"
    :style="{ backgroundImage: `url(${heroImage})` }"
  >
    <section
      class="sm:mb-8 mx-auto flex sm:flex-row flex-col sm:justify-center"
    >
      <div class="container text-start">
        <h1 class="title uppercase text-blue-950">logic lab</h1>
        <span class="text-orange-500 font-bold capitalize"
          >think, code, create!</span
        >
        <p class="subtitle text-black">
          Kami adalah komunitas belajar IT yang juga menyediakan layanan
          professional dalam pengembangan web, desain UI/UX, dan konsultasi
          teknologi
        </p>
        <div class="mt-10 items-center gap-x-6">
          <a
            href="#"
            class="rounded-full bg-blue-800 px-9 py-2 text-sm font-semibold text-gray-300 hover:bg-gray-700 hover:text-white"
            >Layanan</a
          >
          <a
            href="#"
            class="rounded-full outline-3 outline-blue-950 px-9 py-2 text-sm font-semibold text-blue-950 hover:bg-gray-700 hover:text-white"
            >Komunitas</a
          >
        </div>
      </div>
    </section>
  </main>
</template>
<style scoped>
@import url(../../tailwindcss/input.css);
@import url(../../tailwindcss/output.css);
</style>
