<template>
  <div
    class="text-sm lg:text-base px-3 py-1 mr-1 sm:mr-2 mt-3 rounded-full inline-block tracking-wide shadow"
  >
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    type: {
      type: String,
      default: 'none',
    },
  },
};
</script>
