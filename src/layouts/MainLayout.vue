<template>
  <q-layout :class="$q.screen.gt.xs ? 'q-pa-lg' : 'q-pa-md'">
    <div class="row align-center justify-between">
      <div class="row align-center items-center">
        <q-icon
          name="menu"
          class="color-primary-blue q-mr-md"
          v-if="$q.screen.lt.sm"
          size="sm"
          @click="toggleMenuBar"
        />
        <img src="~assets/CodersCommunity.svg" width="250" />
      </div>
      <div class="row align-center justify-center items-center">
        <q-icon
          name="search"
          size="md"
          class="color-primary-blue cursor-pointer"
          v-if="$q.screen.gt.xs"
        ></q-icon>
        <q-avatar
          rounded
          icon="person_outline"
          size="lg"
          class="color-primary-blue"
          v-if="$q.screen.lt.sm"
        />
        <q-btn
          v-else
          flat
          border
          no-caps
          class="color-primary-blue q-ml-md q-px-lg fw-500 fs-16 bg-secondary-blue login-button"
        >
          Login
        </q-btn>
      </div>
    </div>
    <q-drawer
      v-model="isMenuOpen"
      show-if-above
      bordered
      v-if="$q.screen.lt.sm"
    >
      <div class="color-primary-blue q-pt-lg q-pl-lg fw-700">
        { CODERS COMMUNITY }
      </div>
      <q-list class="q-pa-md">
        <!-- <q-item class="fw-500">Home</q-item>
        <q-item class="fw-500">Explore Groups</q-item>
        <q-item class="fw-500">Events</q-item>
        <q-item class="fw-500">Trending</q-item>
        <q-item class="fw-500">Search</q-item> -->
        <q-item class="fw-500 menu-items row align-center items-center">
          <q-icon name="home" class="q-pr-sm" size="xs" />
          <div>Home</div>
        </q-item>
        <q-item class="fw-500 menu-items row align-center items-center">
          <q-icon name="find_in_page" class="q-pr-sm" size="xs" />
          <div>Explore Groups</div>
        </q-item>
        <q-item class="fw-500 menu-items row align-center items-center">
          <q-icon name="event" class="q-pr-sm" size="xs" />
          <div>Events</div>
        </q-item>
        <q-item class="fw-500 menu-items row align-center items-center">
          <q-icon name="trending_up" class="q-pr-sm" size="xs" />
          <div>Trending Tags</div>
        </q-item>
        <q-item class="fw-500 menu-items row align-center items-center">
          <q-icon name="search" class="q-pr-sm" size="xs" />
          <div>Search</div>
        </q-item>
      </q-list>
    </q-drawer>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainLayout",
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenuBar() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
});
</script>

<style lang="scss" scoped>
.login-button {
  border-radius: 20px;
  border: solid 1px $primary-blue;
}
.menu-items :hover {
  color: $primary-blue;
}
</style>
