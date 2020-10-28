<template>
  <div class="flex items-start">
    <div class="flex-shrink-0 inline-flex items-center">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        class="mt-1 xl:mt-2 h-4 w-4 text-secondary inline"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M9 5l7 7-7 7"
        />
      </svg>
    </div>
    <div class="pl-1">
      <div :style="marginTop">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    size: {
      type: String,
      default: 'normal',
    },
  },
  computed: {
    marginTop() {
      switch (this.$props.size) {
        case 'small':
          return 'margin-top: 0.3rem';
        case 'large':
          return 'margin-top: 0rem';
        default:
          return 'margin-top: 0.15rem';
      }
    },
  },
};
</script>
