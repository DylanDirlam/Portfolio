<template>
  <div class="inline">
    <div class="hidden md:inline-block zoom">
      <NuxtLink
        :to="to"
        class="mx-2 px-2 lg:px-4 py-2 bg-transparent md:text-lg text-white"
      >
        <slot></slot>
      </NuxtLink>
    </div>
    <div
      class="inline-block md:hidden px-4 py-4 w-full text-2xl"
      @click="hideMenu()"
    >
      <NuxtLink :to="to" class="px-4 py-4">
        <slot></slot>
      </NuxtLink>
    </div>
  </div>
</template>

<script>
import { HideMenuEventBus } from './Navbar';
export default {
  props: {
    to: {
      type: String,
      default: '404',
    },
  },
  methods: {
    hideMenu() {
      HideMenuEventBus.$emit('hide-menu');
    },
  },
};
</script>
