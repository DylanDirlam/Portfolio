<template>
  <div
    class="flex flex-col w-full min-h-screen h-full font-body bg-gradient-to-b from-blue-900 to-teal-700 overflow-x-hidden"
  >
    <Navbar />
    <main class="flex-grow mt-16 md:mt-0">
      <Nuxt />
    </main>
    <Footer />
  </div>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';
AOS.init();
export default {
  created() {
    AOS.init({
      duration: 1000,
    });
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
</style>
