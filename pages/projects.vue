<template>
  <div class="flex align-middle h-full text-white py-6">
    <div class="container mx-auto px-4 md:px-0 md:w-4/5">
      <ProjectCard
        title="Municipality Management"
        link="https://cmm.compassweb.dev/"
        created-text="Released "
        year="Dec 2021"
        data-aos="fade-left"
        image="cmm.jpg"
        highlight
      >
        <template #description>
          <Arrow>
            Tool created for site administrators to be able to manage
            many sites through a convenient portal.
          </Arrow>

          <Arrow>
            Allows site managers to upload notices, minutes, agendas,
            resolutions, and other files required by law.
          </Arrow>

          <Arrow>
            Utilizes Amazon AWS S3 buckets to store and serve files.
          </Arrow>

          <Arrow>
            Over 50 municipal organizations using the platform!
          </Arrow>
        </template>
        <template #techstack>
          <InertiaPill />
          <ReactPill />
          <LaravelPill />
        </template>
      </ProjectCard>
      <ProjectCard
        title="Digitell DX Platform"
        link="https://www.digitell.tv/"
        created-text="Joined project in"
        year="2021"
        data-aos="fade-right"
        image="opus.jpg"
        highlight
      >
        <template #description>
          <Arrow>
            Rewrote image manipulation to allow users to crop and
            rotate their images in the browser. Resizing is done using
            using JavaScript within the browser before being sent to
            the server, thus saving time and resources.
          </Arrow>

          <Arrow>
            Built reports for clients to track their event
            performances.
          </Arrow>

          <Arrow>
            Created tools for conference attendees to network and
            connect.
          </Arrow>

          <Arrow>
            Created tools to allow conference exhibitors to showcase
            their virtual booths.
          </Arrow>

          <Arrow>
            Created REST API endpoints to support client application
            integrations with the platform.
          </Arrow>
        </template>
        <template #techstack>
          <BootstrapPill />
          <PhpPill />
          <FuelPhpPill />
          <MySqlPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="WoWAnalyzer"
        link="https://www.wowanalyzer.com/"
        github="https://github.com/WoWAnalyzer/WoWAnalyzer"
        created-text="Joined project in"
        year="2020"
        data-aos="fade-left"
        image="wowanalyzer.jpg"
      >
        <template #description>
          <Arrow>
            Converted JavaScript components and files to TypeScript.
          </Arrow>

          <Arrow>
            Developed modules to support in-depth analysis of World of
            Warcraft player performance.
          </Arrow>

          <Arrow>
            Provided code reviews for pull requests from new members
            to the project.
          </Arrow>
        </template>
        <template #techstack>
          <TypeScriptPill />
          <ReactPill />
          <JestPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="Saxon Glass Website"
        link="https://www.saxonglass.com/"
        year="2020"
        data-aos="fade-right"
        image="saxon.jpg"
        highlight
      >
        <template #description>
          <Arrow>
            Redesigned company website to highlight the products and
            services offered by the business.
          </Arrow>

          <Arrow>
            Photographed products and equipment in the factory. 👨‍🔬
          </Arrow>
        </template>
        <template #techstack>
          <VuePill />
          <NuxtjsPill />
          <TailwindCssPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="Portfolio Website"
        link="https://www.dirlam.dev/"
        github="https://github.com/DylanDirlam/Portfolio"
        year="2020"
        data-aos="fade-left"
        image="portfolio.jpg"
      >
        <template #description>
          <Arrow>
            Portfolio website to show a bit about me, my resume, and
            previous projects I've worked on.
          </Arrow>

          <Arrow> It's the site you're on right now! 🥳 </Arrow>
        </template>
        <template #techstack>
          <VuePill />
          <NuxtjsPill />
          <TailwindCssPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="Saxon MessageBoard"
        year="2018"
        data-aos="fade-right"
        image="messageboard.jpg"
      >
        <template #description>
          <Arrow>
            Web app built as an internal HR tool to send out text,
            email, and phone calls to employees using
            <a
              href="https://twilio.com"
              rel="noreferrer"
              target="_blank"
              class="text-blue-400 hover:underline hover:text-blue-600"
              >Twilio API</a
            >.
          </Arrow>

          <Arrow>
            Training management to track employees' training status
            and expiration dates; notify management when an employee
            is due for a recurring training.
          </Arrow>

          <Arrow>
            Calendar to track recurring maintenances for factory
            items; notify management when due for maintenance. 🛠
          </Arrow>
        </template>
        <template #techstack>
          <BootstrapPill />
          <PhpPill />
          <TwilioPill />
          <MySqlPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="Town of Friendship, NY"
        link="https://www.townoffriendship-ny.com/"
        year="2017"
        data-aos="fade-right"
        image="friendship.jpg"
      >
        <template #description>
          <Arrow>
            Mobile-responsive site built with
            <a
              href="https://getbootstrap.com/"
              rel="noreferrer"
              target="_blank"
              class="text-blue-400 hover:underline hover:text-blue-600"
              >Bootstrap</a
            >
            for the Town of Friendship.
          </Arrow>

          <Arrow>
            PHP back-end with a login and simple form; allows town
            officials to easily add meeting minutes, agendas,
            resolutions, and yearly budgets. This has allowed the site
            to be run with minimal maintenance for many years.
          </Arrow>

          <Arrow>
            Photographed the town and its landmarks to use on the
            site. 📷
          </Arrow>
        </template>
        <template #techstack>
          <BootstrapPill />
          <PhpPill />
          <MySqlPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="Saxon Sheets"
        year="2016"
        data-aos="fade-left"
        image="saxon_sheets.jpg"
        highlight
      >
        <template #description>
          <Arrow>
            Web app built as an internal tool to track and manage
            factory production from receiving, processing, and
            shipping.
          </Arrow>

          <Arrow>
            Tracks employee productivity and tasks that were completed
            day-to-day; provides reports for daily, weekly, monthly,
            yearly performance.
          </Arrow>

          <Arrow>
            Audits factory functions to ensure everything is done
            according to procedure. 📝
          </Arrow>

          <Arrow>
            Much, much more that cannot fit in this small blurb.
          </Arrow>
        </template>
        <template #techstack>
          <BootstrapPill />
          <PhpPill />
          <MySqlPill />
        </template>
      </ProjectCard>

      <ProjectCard
        title="Wellsville Airport"
        link="https://www.wellsvilleairport.com/"
        year="2016"
        data-aos="fade-left"
        image="wellsville-airport.jpg"
      >
        <template #description>
          <Arrow>
            Mobile-responsive site built with
            <a
              href="https://getbootstrap.com/"
              rel="noreferrer"
              target="_blank"
              class="text-blue-400 hover:underline hover:text-blue-600"
              >Bootstrap</a
            >
            for the Wellsville Airport.
          </Arrow>

          <Arrow>
            Simple login made with PHP; allows the airport supervisor
            to update prices for fuel.
          </Arrow>

          <Arrow>
            Photographed the airport and airplanes to use on the site.
            📷
          </Arrow>
        </template>
        <template #techstack>
          <BootstrapPill />
          <PhpPill />
          <MySqlPill />
        </template>
      </ProjectCard>
    </div>
  </div>
</template>
