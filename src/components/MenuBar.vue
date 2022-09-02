<template>
  <div>
    <div class="q-mt-xl menu-conatiner">
      <div
        class="row align-center items-center q-py-sm cursor-pointer menu-items"
      >
        <q-icon name="home" class="q-pr-md" size="sm" />
        <div>Home</div>
      </div>
      <div
        class="row align-center items-center q-py-sm cursor-pointer menu-items"
      >
        <q-icon name="find_in_page" class="q-pr-md" size="sm" />
        <div>Explore Groups</div>
      </div>
      <div
        class="row align-center items-center q-py-sm cursor-pointer menu-items"
      >
        <q-icon name="event" class="q-pr-md" size="sm" />
        <div>Events</div>
      </div>
    </div>
    <div class="tags-container q-mt-lg">
      <div class="row align-center items-center">
        <div class="fw-500 fs-16 q-mr-sm">Trending Tags</div>
        <q-icon name="trending_up" size="sm"></q-icon>
      </div>
      <div class="q-mt-sm">
        <div class="tags-item cursor-pointer q-py-xs">
          <span>#javascript</span>
        </div>
        <div class="tags-item cursor-pointer q-py-xs">
          <span>#pythondevelopment</span>
        </div>
        <div class="tags-item cursor-pointer q-py-xs">
          <span>#vue</span>
        </div>
        <div class="tags-item cursor-pointer q-py-xs">
          <span>#100daysofcode</span>
        </div>
        <div class="tags-item cursor-pointer q-py-sm fw-500">
          <span>View all</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuBar",
};
</script>

<style lang="scss" scoped>
.menu-conatiner {
  border-radius: 10px;
  border: solid 0.5px rgba(0, 0, 0, 0.25);
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  padding: 20px;
}

.menu-items :hover {
  color: $primary-blue;
}
.tags-item :hover {
  color: $primary-blue;
}
.tags-container {
  border-radius: 10px;
  border: solid 0.5px rgba(0, 0, 0, 0.25);
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  padding: 20px;
}
</style>
