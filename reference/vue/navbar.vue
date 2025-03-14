<script setup>
import { ref } from "vue";

const isMobileMenuOpen = ref(false);

const toggleMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};
</script>
<template>
  <nav class="navbar bg-white shadow-md shadow-gray-500 has-outline">
    <div class="navbar-brand items-center sm:items-stretch sm:justify-center">
      <div class="flex shrink-0 items-center">Logic Lab</div>
    </div>
    <!-- Mobile menu -->
    <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
      <button
        type="button"
        @click="toggleMenu"
        class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-700 hover:bg-blue-950 hover:text-blue-950 focus:ring-2 focus:ring-white focus:outline-hidden focus:ring-inset"
        aria-controls="mobile-menu"
        aria-expanded="false"
      >
        <span class="absolute -inset-0.5"></span>
        <span class="sr-only">Open main menu</span>

        <svg
          v-if="!isMobileMenuOpen"
          class="block size-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          aria-hidden="true"
          data-slot="icon"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
          />
        </svg>

        <svg
          v-else
          class="hidden size-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          aria-hidden="true"
          data-slot="icon"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6 18 18 6M6 6l12 12"
          />
        </svg>
      </button>
    </div>
    <!-- Desktop menu -->
    <menu class="navbar-menu">
      <div class="hidden sm:block">
        <div class="navbar-buttons">
          <a
            href="#home"
            class="navbar-item text-gray-700 hover:text-blue-950"
            aria-current="page"
            >Beranda</a
          >
          <a
            href="#service"
            class="navbar-item text-gray-700 hover:text-blue-950"
            >Layanan</a
          >
          <a
            href="#aboutUs"
            class="navbar-item text-gray-700 hover:text-blue-950"
            >Tentang</a
          >
          <a href="#" class="navbar-item text-gray-700 hover:text-blue-950"
            >Desain</a
          >
          <a
            href="#"
            class="rounded-full bg-blue-800 px-9 py-2 text-sm font-medium text-gray-300 hover:bg-gray-700 hover:text-white"
            >Kirim Pesan</a
          >
        </div>
      </div>
    </menu>

    <!-- Mobile Menu -->
    <div class="sm:hidden" id="mobile-menu" v-if="isMobileMenuOpen">
      <div class="space-y-1 px-2 pt-2 pb-3">
        <a
          href="#"
          class="block rounded-md bg-gray-900 px-3 py-2 text-base font-medium text-white"
          aria-current="page"
          >Beranda</a
        >
        <a
          href="#"
          class="block rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-gray-700 hover:text-white"
          >Layanan</a
        >
        <a
          href="#"
          class="block rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-gray-700 hover:text-white"
          >Tentang</a
        >
        <a
          href="#"
          class="block rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-gray-700 hover:text-white"
          >Desain</a
        >
      </div>
    </div>

    <!-- Search Button -->
    <div
      class="absolute inset-y-0 right-0 flex pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-1"
    >
      <button
        type="button"
        class="relative rounded-full bg-blue-500 hover:text-blue-950 p-1 text-blue-400 focus:outline-hidden focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
      >
        <span class="absolute -inset-1.5"></span>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-6 h-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z"
          />
        </svg>
      </button>
    </div>
  </nav>
</template>
<style scoped>
@import url(../../tailwindcss/input.css);
@import url(../../tailwindcss/output.css);
</style>
