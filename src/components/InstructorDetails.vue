<template>
  <div class="q-mt-xl">
    <div class="text-center fw-700 fs-32 linear-color">Meet our Hero!</div>
    <div class="row justify-center q-mt-lg">
      <div class="col-md-4 col-sm-12 col-xs-12">
        <img src="~assets/instructor.webp" alt="" />
      </div>
      <div class="col-md-6 col-sm-12 col-xs-12 q-ml-md q-mt-sm">
        <div class="fs-24 fw-600">John Doe</div>
        <em>-Software Engineer</em>
        <div class="fs-20">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam, quia
          aliquid veniam ad praesentium maiores quibusdam tenetur error
          aspernatur veritatis reprehenderit atque vel accusantium, rem.
        </div>
        <div class="row q-mt-lg">
          <div
            class="social-media-container cursor-pointer q-mt-sm"
            id="linkedin"
          >
            <i class="fa-brands fa-linkedin"></i>
          </div>
          <div
            class="social-media-container cursor-pointer q-mt-sm"
            id="github"
          >
            <i class="fa-brands fa-github"></i>
          </div>
          <div
            class="social-media-container cursor-pointer q-mt-sm"
            id="facebook"
          >
            <i class="fa-brands fa-facebook-f"></i>
          </div>
          <div
            class="social-media-container cursor-pointer q-mt-sm"
            id="instagram"
          >
            <i class="fa-brands fa-instagram"></i>
          </div>
          <div
            class="social-media-container cursor-pointer q-mt-sm"
            id="youtube"
          >
            <i class="fa-brands fa-youtube"></i>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InstructorDetails",
};
</script>

<style lang="scss" scoped>
img {
  width: 100%;
  max-width: 350px;
  height: 250px;
  border-radius: 20px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  @media only screen and (max-width: $breakpoint-sm-max) {
    max-width: 350px;
    display: block;
    margin-left: auto;
    margin-right: auto;
    height: 250px;
    object-fit: fill;
  }
  @media only screen and (max-width: $breakpoint-xs-max) {
    max-width: 100%;
    height: auto;
  }
}
i {
  font-size: 28px;
}
.social-media-container {
  border-radius: 5px;
  margin-right: 20px;
  padding: 5px 10px;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
</style>
