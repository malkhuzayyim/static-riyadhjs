<template>
  <div id="riyadhjs" class="py-12 px-1">
    <div class="display-3 py-1">
      <span class="ubunto">
        Riyadh JS
      </span>
    </div>
    <div class="subtitle-1 py-1">
      On a mission to unite the javascript &amp; web development community in
      Riyadh, Saudi Arabia.
    </div>
    <div class="subtitle-1 py-1">
      This is a brand new initiative, as of November 2019.
    </div>
    <content-card id="brief">
      <template #title>
        A brief
      </template>
      <template #body>
        The reason we're starting this is to help build a community for us, the
        javascript enthusiasts, so we get visibility on who's out there doing
        similar work, connect with them, collaborate, and share experiences.
      </template>
    </content-card>
    <content-card id="audience">
      <template #title>
        Target Audience
      </template>
      <template #body>
        People who're already working (or studying) in the web development
        space, and are interested in Javascript &amp; its ecosystem of
        technologies.
      </template>
    </content-card>
    <content-card id="frequency">
      <template #title>
        Meetups Frequency
      </template>
      <template #body>
        The current idea is to have a monthly meetup, the first Saturday of
        every month, at 4pm.
      </template>
    </content-card>
    <content-card id="format">
      <template #title>
        Meetups Format
      </template>
      <template #body>
        We hope to have each meetup structured as follows:
        <br />
        - 20-30 minutes where we'll have a pre-determined speaker cover a
        topic/technology of interest, with an interesting demo or something of
        the sort.
        <br />
        - 10-15 minutes of Q&amp;A regarding the topic at hand.
        <br />
        - Freeform discussion on whatever comes to mind &amp; planning the next
        meetup.
      </template>
    </content-card>
    <content-card id="venue">
      <template #title>
        Meetups Venue
      </template>
      <template #body>
        We've discussed this with
        <a href="https://astrolabs.com" target="_blank">
          Astrolabs
        </a>
        and they're willing to provide a venue for the meetups, free of charge.
        <br />
        <br />
        Their Riyadh location can be found here:
        <br />
        <a
          href="https://www.google.ae/maps/place/%D8%A3%D8%B3%D8%AA%D8%B1%D9%88%D9%84%D8%A7%D8%A8%D8%B2%E2%80%AD/@24.8064543,46.6150945,21z/data=!4m5!3m4!1s0x3e2ee5973ff30251:0xe165035711dcf14f!8m2!3d24.8064668!4d46.6151907"
        >
          Google Maps Link
        </a>
      </template>
    </content-card>
    <content-card id="scope">
      <template #title>
        Meetups Scope
      </template>
      <template #body>
        The following is a list of technologies that we believe should be the
        focus of this initiative:
        <br />
        - Javascript Frontend Technologies (Mainly Vue &amp; React)
        <br />
        - NodeJS API Development (REST API's &amp; GraphQL)
        <br />
        - Databases (Can't do much without one)
        <br />
        - Deployment Solutions &amp; Platforms (think AWS, Heroku, Netlify,
        etc.)
        <br />
        - Git &amp; Github Workflows
        <br />
        - Javascript Hybrid Development (Mobile &amp; Desktop apps)
        <br />
        <br />
        This is not an exhaustive list, but you get the gist of where we're
        going with this.
        <br />
        <br />
        The idea is that most topics &amp; discussions should be related to
        modern tech stacks in the Javascript Ecosystem.
      </template>
    </content-card>
    <content-card id="team">
      <template #title>
        RiyadhJS Team - Looking for Help
      </template>
      <template #body>
        The person starting this (myself) is Mohammed Alkhuzayyim, an Industrial
        Engineer turned web developer, with a focus on Fullstack Javascript web
        development. My favorite techstack is comprised of: PostgreSQL, Express,
        Node, Vue, Vuetify.
        <br />
        <br />
        I'm looking for people to help me scope this out further &amp; organize
        it.
        <br />
        <br />
        If you're interested, please fill out this small form:
        <a href="" target="_blank">
          Apply to be a Riyadh JS Core Member
        </a>
      </template>
    </content-card>
  </div>
</template>

<script>
import ContentCard from "@@/components/ContentCard";
export default {
  components: {
    "content-card": ContentCard
  }
};
</script>
