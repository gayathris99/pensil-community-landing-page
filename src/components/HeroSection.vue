<template>
  <div
    class="row align-center"
    :class="$q.screen.width >= 1024 ? 'justify-evenly' : ''"
  >
    <div class="q-mx-auto" v-if="$q.screen.width < 1024">
      <img src="~assets/heroimage.webp" />
    </div>
    <div class="col-8" :class="{ 'q-mx-auto': $q.screen.width < 1024 }">
      <div class="fw-700 fs-36 q-mt-xl">
        <span class="linear-color">Community</span> for brilliant
        <br />
        coders like you.
      </div>
      <div class="fw-500 q-mt-md fs-16">
        Get help from any corner of the world
      </div>
      <q-btn
        label="Become an active member today"
        rounded
        no-caps
        style="
          background: -webkit-linear-gradient(#5b86e5, #36d1dc);
          color: white;
        "
        class="q-mt-xl fw-500 fs-20 q-py-sm q-px-md"
      />
    </div>
    <div class="col-4 q-ml-md" v-if="$q.screen.width >= 1024">
      <img src="~assets/heroimage.webp" />
    </div>
  </div>
</template>

<script>
export default {
  name: "HeroSection",
};
</script>

<style lang="scss" scoped>
.linear-color {
  background: -webkit-linear-gradient(#5b86e5, #36d1dc);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.linear-color-btn {
  color: #5b86e5;
}
img {
  width: 100%;
  max-width: 400px;
  @media only screen and (max-width: 1023px) {
    max-width: 300px;
  }
}
</style>
