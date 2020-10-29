<template>
  <div
    class="flex align-middle h-full text-white pt-8 pb-6 md:py-10 xl:py-12"
  >
    <div class="md:container mx-auto">
      <div
        class="md:ml-12 lg:ml-48 md:flex md:flex-row pb-6 md:pb-12"
      >
        <img
          src="~/assets/self.jpg"
          width="800"
          height="800"
          alt="Picture of my face"
          class="mx-auto w-1/2 h-1/2 rounded-full shadow-xl"
          data-aos="fade-right"
        />
        <div
          class="text-center md:text-left mx-auto w-2/3 mt-auto pt-6 md:pt-0 pb-4 md:pb-12 md:-ml-12 lg:-ml-48 z-10"
        >
          <h1
            class="pb-2 md:pb-0 text-2xl lg:text-6xl"
            data-aos="fade-left"
            data-aos-delay="200"
          >
            Hi, I'm
            <span class="text-secondary font-semibold"
              >Dylan Dirlam</span
            >.
          </h1>
          <h2
            class="text-xl lg:text-3xl"
            data-aos="fade-left"
            data-aos-delay="400"
          >
            I'm a
            <span class="text-secondary">Software Developer</span>
            with a passion for building web apps to power businesses.
          </h2>
        </div>
      </div>
      <div class="flex w-full">
        <NuxtLink
          to="/projects"
          class="text-secondary mx-auto text-lg md:text-xl rounded-full border border-secondary px-4 py-2 flex items-center md:tracking-wide zoom"
        >
          View my Projects
        </NuxtLink>
      </div>
    </div>
  </div>
</template>
