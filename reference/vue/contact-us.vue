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
      <section id="contactUs" class="isolate bg-white px-6 py-24 sm:py-32 lg:px-8">
        <div class="mx-auto container text-center">
            <h1 class="title text-balance text-gray-900 mb-8"><span class="capitalize">ayo</span> hubungi kami</h2>
                <p class="subtitle text-gray-600 mb-8"><span class="capitalize">ada</span> yang mau disampaikan atau
                    ditanyakan? Yuk langsung hubungi kami</p>
        </div>
        <form action="#" method="POST" class="mx-auto mt-10 max-w-md sm:mt-20 justify-self-center justify-items-center">
            <div class="container grid grid-cols-1 gap-x-8 gap-y-6 sm:grid-cols-2">
                <div>
                    <!-- Name -->
                    <div class=" mt-2.5 relative flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="absolute  w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M15.75 6a3.75 3.75 0 1 1-7.5 0 3.75 3.75 0 0 1 7.5 0ZM4.501 20.118a7.5 7.5 0 0 1 14.998 0A17.933 17.933 0 0 1 12 21.75c-2.676 0-5.216-.584-7.499-1.632Z" />
                        </svg>
                        <input type="text" name="name" id="name" autocomplete="name" placeholder="Nama"
                            class="block w-full rounded-md bg-white px-3.5 py-2 text-base text-gray-900 shadow-sm placeholder:text-gray-400 focus:outline-2 focus:-outline-offset-2 focus:bg-blue-800">
                    </div>
                </div>
                <!-- No Telepon -->
                <div class="relative flex items-center">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="absolute w-6 h-6">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 0 0 2.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 0 1-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 0 0-1.091-.852H4.5A2.25 2.25 0 0 0 2.25 4.5v2.25Z" />
                    </svg>
                    <input type="tel" name="no_telp" id="no_telp" autocomplete="cc-number" placeholder="No Telepon"
                        class="block w-full rounded-md bg-white px-3.5 py-2 text-base text-gray-900 shadow-sm placeholder:text-gray-400 focus:outline-2 focus:-outline-offset-2 focus:bg-blue-800">
                </div>
                <!-- email -->
                <div class="sm:col-span-2">
                    <div class="relative flex items-center">
                        <input type="email" name="email" id="email" autocomplete="email" placeholder="Email"
                            class="block w-full rounded-md bg-white px-3.5 py-2 text-base text-gray-900 shadow-sm placeholder:text-gray-400 focus:outline-2 focus:-outline-offset-2 focus:bg-blue-800">

                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="absolute w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M21.75 6.75v10.5a2.25 2.25 0 0 1-2.25 2.25h-15a2.25 2.25 0 0 1-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0 0 19.5 4.5h-15a2.25 2.25 0 0 0-2.25 2.25m19.5 0v.243a2.25 2.25 0 0 1-1.07 1.916l-7.5 4.615a2.25 2.25 0 0 1-2.36 0L3.32 8.91a2.25 2.25 0 0 1-1.07-1.916V6.75" />
                        </svg>

                    </div>
                </div>
                <!-- Pesan -->
                <div class="sm:col-span-2">
                    <div class="relative flex items-start">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                            stroke="currentColor" class="absolute w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M12 20.25c4.97 0 9-3.694 9-8.25s-4.03-8.25-9-8.25S3 7.444 3 12c0 2.104.859 4.023 2.273 5.48.432.447.74 1.04.586 1.641a4.483 4.483 0 0 1-.923 1.785A5.969 5.969 0 0 0 6 21c1.282 0 2.47-.402 3.445-1.087.81.22 1.668.337 2.555.337Z" />
                        </svg>
                        <textarea name="message" id="message" rows="4" placeholder="Pesan"
                            class="inline w-full rounded-md bg-white p-2.5 pl-10 text-base text-gray-900 shadow-sm placeholder:text-gray-400 focus:outline-2 focus:-outline-offset-2 focus:bg-blue-800"
                            required></textarea>
                    </div>
                </div>
            </div>
            <div class="mt-3">
                <button type="submit"
                    class="rounded-full bg-blue-800 px-12 py-3 text-sm font-semibold text-gray-300 hover:bg-gray-700 hover:text-white">Kirim</button>
            </div>
        </form>
    </section>

</template>
<style scoped>
@import url(../../tailwindcss/input.css);
@import url(../../tailwindcss/output.css);
</style>
