<script>
export default {
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <header>
    <div class="center header-height">
      <div class="container h-100 spaced-centered-divs">
        <div class="h-100">
          <div class="h-100 centered-vertically-div">
            <img class="h-75" src="../assets/img/dc-logo.png" alt="" />
          </div>
        </div>
        <div>lol</div>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/mixins.scss" as *;
.header-height {
  height: $header_height;
}
.h-75 {
  height: 75%;
}
</style>
