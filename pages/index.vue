<template>
  <div id="riyadhjs" class="py-12 px-1">
    <div class="display-3 py-1">
      <span class="ubunto">
        Riyadh JS
      </span>
    </div>
    <div class="subtitle-1 py-1">
      A meetup for all things JS.
      <br />
      Located in Riyadh, Saudi Arabia.
    </div>
    <div class="text-right">
      <v-btn @click="toHash(`team`)" color="primary">
        Join the team
      </v-btn>
    </div>
    <content-card id="intro">
      <template #title>
        Intro
      </template>
      <template #body>
        The reason we're starting this is to help build a community for people
        working in the web development space in Riyadh, Saudi Arabia. To
        connect, collaborate, and share experiences.
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
        We hope to be consistent with our meetups, about once a month.
      </template>
    </content-card>
    <content-card id="format">
      <template #title>
        Meetups Format
      </template>
      <template #body>
        Each meetup would roughly last an hour, and will consist of a primary
        topic, which will be covered by a speaker for in the first half hour.
        The second half will usually be a free-format discussion.
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
        modern tech stacks in the Web Development Ecosystem.
      </template>
    </content-card>
    <content-card id="team">
      <template #title>
        RiyadhJS Team
      </template>
      <template #body>
        <div class="pb-3">
          As of now it's a team of one.
          <br /><br />
          - Mohammed Alkhuzayyim
          <br /><br />
          This is just getting started, if you'd like to be involved, please
          feel free to introduce yourself by emailing me at
          <a href="mailto:m.alkhuzayyim@gmail.com">
            m.alkhuzayyim@gmail.com
          </a>
        </div>
      </template>
    </content-card>
  </div>
</template>

<script>
import ContentCard from "@@/components/ContentCard";
export default {
  components: {
    "content-card": ContentCard
  },
  methods: {
    toHash(hash) {
      this.$vuetify.goTo(`#${hash}`, {
        duration: 500,
        offset: 50,
        easing: "easeInOutCubic"
      });
    }
  }
};
</script>
