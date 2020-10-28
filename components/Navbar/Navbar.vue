<template>
  <div class="w-full">
    <div
      class="hidden md:flex md:container md:mx-auto w-full z-100 p-8 flex-row items-center"
    >
      <div class="flex-auto">
        <NuxtLink to="/">
          <h1 class="text-white text-xl sm:text-3xl lg:text-5xl">
            Dylan Dirlam
          </h1>
        </NuxtLink>
      </div>
      <div
        class="py-4 lg:py-8 px-2 lg:px-5 rounded-full transition-opacity duration-700 bg-gray-800"
      >
        <NavLink to="/">Home</NavLink>
        <NavLink to="/projects">Projects</NavLink>
        <NavLink to="/about">About Me</NavLink>
        <NavLink to="/contact">Contact</NavLink>
      </div>
    </div>
    <div
      :class="[
        'z-0 fixed top-0 left-0 bg-black w-full h-screen transition duration-700 ease-in-out',
        mobileMenuOpen
          ? 'opacity-75'
          : 'opacity-0 pointer-events-none',
      ]"
      @click="mobileMenuOpen = false"
    ></div>
    <div class="md:hidden fixed w-full z-100 pointer-events-none">
      <div
        class="w-full flex items-center md:hidden z-100 bg-gradient-to-l from-blue-800 to-teal-700 text-white px-6 py-4 pointer-events-auto"
      >
        <div class="flex-auto">
          <NuxtLink to="/">
            <h1 class="text-2xl text-white">Dylan Dirlam</h1>
          </NuxtLink>
        </div>
        <div class="justify-end">
          <a role="button" @click="mobileMenuOpen = !mobileMenuOpen">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              class="w-8 h-8 text-white"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </a>
        </div>
      </div>
      <div
        :class="[
          `flex w-1/2 bg-gray-800 bg-opacity-75 min-h-screen h-full text-white transition-opacity duration-500 ease`,
          mobileMenuOpen
            ? 'opacity-100 pointer-events-auto'
            : 'opacity-0 pointer-events-none',
        ]"
      >
        <div class="mt-12" @hide-menu="mobileMenuOpen = false">
          <NavLink to="/">Home</NavLink>
          <NavLink to="/projects">Projects</NavLink>
          <NavLink to="/about">About Me</NavLink>
          <NavLink to="/contact">Contact</NavLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
export const HideMenuEventBus = new Vue();
export default {
  data() {
    HideMenuEventBus.$on('hide-menu', () => {
      this.mobileMenuOpen = false;
    });
    return {
      mobileMenuOpen: false,
    };
  },
};
</script>
