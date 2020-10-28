<template>
  <div
    :class="[
      'md:flex md:flex-row mb-6 md:mb-16',
      highlight ? 'border-2 border-secondary rounded-2xl' : '',
    ]"
  >
    <a
      :href="link"
      target="_blank"
      class="md:w-2/5 h-auto w-full overflow-hidden rounded-t-xl md:rounded-t-none md:rounded-l-xl"
    >
      <img
        :src="getImageUrl()"
        :class="[
          'w-full h-full object-cover object-center rounded-t-xl md:rounded-t-none md:rounded-l-xl overflow-hidden',
          link ? 'zoom' : '',
        ]"
      />
    </a>
    <div
      class="md:flex md:flex-col md:w-3/5 px-5 md:px-10 py-6 bg-gray-800 bg-opacity-50 rounded-b-xl md:rounded-b-none md:rounded-r-xl"
    >
      <div class="flex flex-row items-center">
        <h1 class="text-xl lg:text-3xl flex-auto">
          <a v-if="link" :href="link">
            {{ title }}
          </a>
          <span v-else>
            {{ title }}
          </span>
          <small
            class="block xl:inline-block text-base xl:text-lg text-gray-400 font-light"
          >
            Created in {{ year }}
          </small>
        </h1>
        <div class="justify-end flex flex-row space-x-2">
          <a
            v-if="github"
            :href="github"
            target="_blank"
            class="text-gray-300 hover:text-secondary zoom"
          >
            <svg
              fill="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="w-6 h-6"
              viewBox="0 0 24 24"
            >
              <path
                d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"
              />
            </svg>
          </a>
          <a
            v-if="link"
            :href="link"
            target="_blank"
            class="text-gray-300 hover:text-secondary zoom"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              class="w-6 h-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"
              />
            </svg>
          </a>
          <svg
            v-if="highlight"
            class="w-6 h-6 text-secondary"
            xmlns="http://www.w3.org/2000/svg"
            fill="currentColor"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              title="Highlighted Project"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="1"
              d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"
            />
          </svg>
        </div>
      </div>
      <div class="xl:text-lg">
        <slot name="description">No description available</slot>
      </div>
      <div class="mt-auto pt-4">
        <slot name="techstack"></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'No title',
    },
    image: {
      type: String,
      default: '',
    },
    year: {
      type: String,
      default: '2010',
    },
    github: {
      type: String,
      default: null,
    },
    link: {
      type: String,
      default: null,
    },
    highlight: {
      type: Boolean,
      default: false,
    },
  },
  methods: {
    getImageUrl() {
      const image = this.$props.image;
      return require(`~/assets/projects/${image}`);
    },
  },
};
</script>
