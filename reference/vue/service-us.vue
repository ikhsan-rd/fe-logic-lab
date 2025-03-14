<script setup>
import { ref } from "vue";

// const isMobileMenuOpen = ref(false);

// const toggleMenu = () => {
//   isMobileMenuOpen.value = !isMobileMenuOpen.value;
// };
</script>
<template>
  <!-- Service -->
  <section id="Service" class="section bg-blue-800 has-outline">
    <div
      class="container mx-auto max-w-7xl grid lg:grid-cols-2 md:grid-cols-2 gap-10 has-outline"
    >
      <!-- Left Column: Text Content -->
      <div class="text-start">
        <h1 class="title text-orange-400 capitalize">layanan</h1>
        <p class="subtitle text-white">
          Website? Desain? Konsultasi? Hubungi Kami!
        </p>
        <div class="mt-5 flex justify-end">
          <a
            href="#"
            class="inline-block rounded-full bg-white px-6 py-2 text-sm font-semibold text-orange-400 hover:bg-gray-700 hover:text-white transition-colors capitalize"
          >
            lihat selangkapnya
          </a>
        </div>
      </div>

      <!-- Right Column: Image -->
      <div class="flex justify-end">
        <img
          src="../assets/ServiceUs (png).png"
          alt="Service Illustration"
          class="max-w-full h-auto"
        />
      </div>
    </div>
  </section>
  <br />

  <!-- Statistic Section -->
  <section
    class="max-w-7xl rounded-3xl bg-blue-800 py-2.5 justify-self-center mx-auto"
  >
    <div
      class="container grid md:grid-cols-2 lg:grid-cols-4 lg:divide-x-3 lg:divide-solid lg:divide-white lg:py-8 mx-auto max-w-7xl"
    >
      <div class="text-center">
        <h3 class="title font-medium text-white capitalize">2</h3>
        <p class="subtitle text-white">Tahun Pengalaman</p>
      </div>
      <div class="text-center">
        <h3 class="title font-medium text-white capitalize">999+</h3>
        <p class="subtitle text-white">Project Terselesaikan</p>
        <!-- border-l-2 border-solid border-white -->
      </div>
      <div class="text-center">
        <h3 class="title font-medium text-white capitalize">99+</h3>
        <p class="subtitle text-white">Client kami</p>
      </div>
      <div class="text-center">
        <h3 class="title font-medium text-white capitalize">5</h3>
        <p class="subtitle text-white">Team Professional</p>
      </div>
    </div>
  </section>
</template>
<style scoped>
@import url(../../tailwindcss/input.css);
@import url(../../tailwindcss/output.css);
</style>
