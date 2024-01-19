<script>
export default {
  data() {
    return {
      nav: [
        {
          name: "CHARACTERS",
        },
        {
          name: "COMICS",
        },
        {
          name: "MOVIES",
        },
        {
          name: "TV",
        },
        {
          name: "GAMES",
        },
        {
          name: "COLLECTIBLES",
        },
        {
          name: "VIDEOS",
        },
        {
          name: "FANS",
        },
        {
          name: "NEWS",
        },
        {
          name: "SHOPS",
        },
      ],
      is_hovering: null,
    };
  },
  methods: {
    change_is_hovering(i) {
      this.is_hovering = i;
    },
    cancel_hovering(i) {
      this.is_hovering = null;
    },
  },
};
</script>

<template>
  <header>
    <div class="center header-height">
      <div class="h-100 container spaced-centered-divs">
        <div class="h-100">
          <div class="h-100 centered-vertically-div">
            <img class="h-75" src="../assets/img/dc-logo.png" alt="" />
          </div>
        </div>
        <div class="h-100 centered-vertically-div">
          <div
            v-for="(elem, i) in nav"
            class="h-100 centered-vertically-div ps-8 pe-8 smaller with-cursor-pointer"
            @mouseover="change_is_hovering(i)"
            @mouseout="cancel_hovering(i)"
            :class="{ hovering: is_hovering == i }"
          >
            {{ elem.name }}
          </div>
        </div>
      </div>
    </div>
    <div class="jumbo-height"></div>
  </header>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/mixins.scss" as *;
.header-height {
  height: $header_height;
}
.jumbo-height {
  height: $footer_one_height;
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
}
.h-75 {
  height: 75%;
}
.hovering {
  color: $main_two_bg;
  border-bottom: 3px solid $main_two_bg;
}
</style>
