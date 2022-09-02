<template>
  <q-page>
    <div class="row">
      <menu-bar class="col-auto" v-if="$q.screen.gt.xs" />
      <hero-section class="col q-mt-xl q-mx-xl" />
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import MenuBar from "components/MenuBar.vue";
import HeroSection from "components/HeroSection.vue";

export default defineComponent({
  name: "IndexPage",
  components: { MenuBar, HeroSection },
});
</script>
