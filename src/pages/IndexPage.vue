<template>
  <q-page>
    <div class="row">
      <menu-bar class="col-auto" v-if="$q.screen.gt.xs" />
      <div class="col q-mt-xl">
        <hero-section class="q-mx-xl" />
        <why-coder-community />
        <instructor-details />
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import MenuBar from "components/MenuBar.vue";
import HeroSection from "components/HeroSection.vue";
import WhyCoderCommunity from "components//WhyCoderCommunity.vue";
import InstructorDetails from "components/InstructorDetails.vue";

export default defineComponent({
  name: "IndexPage",
  components: { MenuBar, HeroSection, WhyCoderCommunity, InstructorDetails },
});
</script>
