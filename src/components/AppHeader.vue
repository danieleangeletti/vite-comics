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
    };
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
        <div class="h-100 centered-vertically-div">
          <div
            v-for="(elem, i) in nav"
            class="h-100 centered-vertically-div ps-8 pe-8 smaller with-cursor-pointer"
          >
            {{ elem.name }}
          </div>
        </div>
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
.ps-8 {
  padding-left: 8px;
}
.pe-8 {
  padding-right: 8px;
}
.smaller {
  font-size: 0.8em;
}
</style>
