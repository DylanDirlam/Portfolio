<template>
  <section class="text-white">
    <div
      class="container px-5 mt-12 mx-auto flex sm:flex-no-wrap flex-wrap"
    >
      <div
        class="lg:w-2/3 md:w-1/2 rounded-lg overflow-hidden sm:mr-10 p-10 flex items-end justify-start relative"
        data-aos="fade-right"
      >
        <iframe
          width="100%"
          height="100%"
          class="absolute inset-0"
          frameborder="0"
          title="map"
          marginheight="0"
          marginwidth="0"
          scrolling="no"
          src="https://www.google.com/maps/embed?pb=!1m10!1m8!1m3!1d1505414.141891738!2d-78.260422!3d42.528489!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sen!2sus!4v1603770499831!5m2!1sen!2sus"
          style="filter: grayscale(1) contrast(1.2) opacity(0.8)"
        ></iframe>
        <div
          class="bg-gradient-to-br from-blue-800 to-teal-600 rounded-xl relative flex flex-row p-4"
        >
          <div class="w-1/2 mx-2">
            <h2 class="text-white">Email</h2>
            <a class="text-sm" href="mailto:dylan@dirlam.dev"
              >dylan@dirlam.dev</a
            >
          </div>
          <div class="w-1/2 mx-2">
            <h2 class="text-white">Phone</h2>
            <a class="text-sm" href="tel:6072815231"
              >(607) 281-5231</a
            >
          </div>
        </div>
      </div>
      <div
        class="lg:w-1/3 md:w-1/2 flex flex-col md:ml-auto w-full md:py-8 mt-8 md:mt-0"
        data-aos="fade-left"
        data-aos-delay="200"
      >
        <h2 class="text-white text-4xl mb-1 font-medium title-font">
          Contact me
        </h2>
        <p class="leading-relaxed mb-5 text-gray-200">
          I'm always eager to work on new projects in my free time.
          Let's work together!
        </p>
        <form class="flex flex-col" name="contact" method="POST" data-netlify="true">
          <input
            class="bg-opacity-75 rounded border text-gray-900 border-gray-400 focus:outline-none focus:border-indigo-500 text-base px-4 py-2 mb-4"
            placeholder="Name"
            name="Name"
            type="text"
            required
          />
          <input
            class="bg-opacity-75 rounded border text-gray-900 border-gray-400 focus:outline-none focus:border-indigo-500 text-base px-4 py-2 mb-4"
            placeholder="Email"
            name="Email"
            type="email"
            required
          />
          <textarea
            class="bg-opacity-75 rounded border text-gray-900 border-gray-400 focus:outline-none h-32 focus:border-indigo-500 text-base px-4 py-2 mb-4 resize-none"
            name="Message"
            placeholder="Message"
            required
          ></textarea>
          <button
            type="submit"
            class="text-secondary border-2 border-secondary py-2 px-6 focus:outline-none zoom rounded-lg text-lg"
          >
            Submit
          </button>
        </form>
      </div>
    </div>
  </section>
</template>
