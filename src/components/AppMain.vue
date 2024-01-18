<script>
export default {
  data() {
    return {
      main_two_items: [
        {
          img: "./src/assets/img/buy-comics-digital-comics.png",
          item_name: "DIGITAL COMICS",
        },
        {
          img: "./src/assets/img/buy-comics-merchandise.png",
          item_name: "DC MERCHANDISE",
        },
        {
          img: "./src/assets/img/buy-comics-subscriptions.png",
          item_name: "SUBSCRIPTION",
        },
        {
          img: "./src/assets/img/buy-comics-shop-locator.png",
          item_name: "COMIC SHOP LOCATOR",
        },
        {
          img: "./src/assets/img/buy-dc-power-visa.svg",
          item_name: "PC POWER VISA",
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <div class="center main-one-bg main-one-height">
      <div class="h-100 container">
        <div class="h-100 centered-vertically-div">
          <div class="white bigger">Content goes here</div>
        </div>
      </div>
    </div>

    <div class="center main-two-bg main-two-height">
      <div class="h-100 container">
        <div class="h-100 centered-vertically-div">
          <div v-for="(item, i) in main_two_items" class="h-40 grow-one">
            <div class="h-100 center centered-vertically-div">
              <img class="h-100 ps-8 pe-8" :src="item.img" alt="" />
              <div class="white ps-4 pe-4 smaller">DIGITAL COMICS</div>
            </div>
          </div>
        </div>
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
.bigger {
  font-size: 1.4em;
}
.h-40 {
  height: 40%;
}
.grow-one {
  flex-grow: 1;
}
</style>
