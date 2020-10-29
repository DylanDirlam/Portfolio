<template>
  <div class="container mx-auto">
    <div class="w-4/5 mx-auto my-6 md:my-12 text-white">
      <img
        src="~/assets/boat.jpg"
        width="800"
        height="969"
        alt="Picture of me on a boat"
        class="w-full h-64 object-cover object-top md:h-auto md:w-2/5 float-left rounded-2xl shadow-lg mr-6 my-2"
        data-aos="fade-right"
      />
      <h1
        class="text-center sm:text-left text-4xl text-white"
        data-aos="fade-left"
      >
        Hi! 👋
        <span class="block sm:inline"
          >I'm
          <span class="text-secondary font-semibold"
            >Dylan Dirlam</span
          >.</span
        >
      </h1>
      <p
        class="py-2 text-lg"
        data-aos="fade-left"
        data-aos-delay="200"
      >
        I'm a Software Developer with a passion for building modern,
        detailed, intuitive websites and web apps to power businesses.
        I have a strong ability to adapt to new environments and pick
        up languages quickly.
      </p>
      <p class="py-2" data-aos="fade-left" data-aos-delay="250">
        Working at
        <a
          href="https://saxonglass.com/"
          rel="noreferrer"
          target="_blank"
          class="text-blue-300 hover:text-blue-400 hover:underline"
          >Saxon Glass</a
        >, I've spent most of my time building in-depth web apps with
        PHP and Bootstrap to increase the productivity and
        organization within the factory. They have been highlighted in
        the <NuxtLink to="/projects">projects</NuxtLink> section. As
        some side projects at Saxon Glass, I've built the following:
      </p>
      <Arrow size="small" data-aos="fade-left" data-aos-delay="300">
        C# Windows program that queries a MySQL database and displays
        data
      </Arrow>
      <Arrow size="small" data-aos="fade-left" data-aos-delay="350">
        OpenCV Python project that uses a TensorFlow object detection
        model to find cracks and chips in glass cartridges. Scans ~50
        cartridges per second with 99.9% accuracy.
      </Arrow>
      <Arrow size="small" data-aos="fade-left" data-aos-delay="400">
        Node.js server that receives temperature readings and uses
        Twilio API to notify management if temperatures are out of
        bounds.
      </Arrow>
      <p class="py-4" data-aos="fade-left" data-aos-delay="450">
        I like to spend my free time growing my abilities as a
        developer by learning new frameworks and languages. Aside from
        programming, I'm an avid World of Warcraft player, car
        enthusiast, and enjoy taking road trips. I've travelled from
        New York to South Dakota, Wyoming, Utah, Maine, and more. Put
        on some good music and I can drive for hours.
      </p>
      <h2
        class="text-center text-xl text-secondary"
        data-aos="fade-up"
        data-aos-delay="500"
      >
        I'm always looking for new opportunities, let's get in touch!
      </h2>
      <div
        class="flex w-full mt-4"
        data-aos="fade-up"
        data-aos-delay="500"
      >
        <a
          target="_blank"
          href="/DylanDirlam_Resume_2020.pdf"
          class="mx-auto px-4 py-2 border-2 text-secondary border-secondary rounded-full text-xl flex items-center zoom"
        >
          View my Resume
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-6 h-6 ml-1"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"
            />
          </svg>
        </a>
      </div>
    </div>
  </div>
</template>
