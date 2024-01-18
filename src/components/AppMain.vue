<script>
export default {
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <main>
    <div class="center main-one-bg main-one-height">
      <div class="container">
        <div>MAIN 1</div>
      </div>
    </div>

    <div class="center main-two-bg main-two-height">
      <div class="container">
        <div>MAIN 2</div>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/mixins.scss" as *;
.main-one-height {
  height: $main_one_height;
}
.main-one-bg {
  background-color: $main_one_bg;
}
.main-two-height {
  height: $main_two_height;
}
.main-two-bg {
  background-color: $main_two_bg;
}
.main-three-bg {
  background-color: black;
}
</style>
