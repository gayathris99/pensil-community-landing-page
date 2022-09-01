<template>
  <q-layout :class="$q.screen.gt.xs ? 'q-pa-lg' : 'q-pa-md'">
    <div class="row align-center justify-between">
      <div class="row align-center justify-start">
        <img src="~assets/CodersCommunity.svg" width="250" />
      </div>
      <div class="row align-center justify-center items-center">
        <q-icon
          name="search"
          size="sm"
          class="color-primary-blue cursor-pointer"
          v-if="$q.screen.gt.xs"
        ></q-icon>
        <q-avatar
          rounded
          icon="person_outline"
          width="40"
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
  </q-layout>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.login-button {
  border-radius: 20px;
  border: solid 1px $primary-blue;
}
</style>
