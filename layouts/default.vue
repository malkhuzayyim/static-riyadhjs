<template>
  <v-app dark>
    <v-app-bar app clipped-left>
      <v-app-bar-nav-icon
        @click="drawer = !drawer"
        class="hidden-lg-and-up"
      ></v-app-bar-nav-icon>
      <v-toolbar-title @click="toHash(`riyadhjs`)" style="cursor: pointer;">
        <span class="ubunto">
          RiyadhJS
        </span>
      </v-toolbar-title>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" app clipped>
      <v-list-item @click="toHash(`riyadhjs`)" link>
        <v-list-item-content>
          <v-list-item-title class="title">
            <span class="ubunto">
              Sections
            </span>
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list nav>
        <v-list-item
          v-for="item in links"
          :key="item.hash"
          @click="toHash(item.hash)"
          :class="item.class"
          link
        >
          <v-list-item-content>
            <v-list-item-title>{{ item.text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-content>
      <v-container style="max-width: 900px;">
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      links: [
        { text: "Intro", hash: "intro", class: "" },
        { text: "Target Audience", hash: "audience", class: "" },
        { text: "Meetups Frequency", hash: "frequency", class: "" },
        { text: "Meetups Format", hash: "format", class: "" },
        { text: "Meetups Venue", hash: "venue", class: "" },
        { text: "Scope", hash: "scope", class: "" },
        {
          text: "Join The Team!",
          hash: "team",
          class: "primary"
        }
      ]
    };
  },
  mounted() {
    if (this.$vuetify.breakpoint.lgAndUp) {
      this.drawer = true;
    }
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

<style>
.ubunto {
  font-family: "Ubuntu Mono", monospace !important;
}
</style>
