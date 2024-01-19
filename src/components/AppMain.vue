<script>
import Card from "./Card.vue";

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
      cards: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "ACTION COMICS",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "AMERICAN VAMPIRE 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "AQUAMAN",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "BATGIRL",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "BATMAN",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$2.99",
          series: "BATMAN BEYOND",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$3.99",
          series: "BATMAN/SUPERMAN",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$4.99",
          series: "BATMAN/SUPERMAN ANNUAL",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "BATMAN: THE JOKER WAR ZONE BATMAN",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "BATMAN: THREE JOKERS",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$4.99",
          series: "BATMAN: WHITE KNIGHT PRESENTS: HARLEY QUINN",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$16.99",
          series: "CATWOMAN",
          type: "graphic novel",
        },
      ],
    };
  },
  components: {
    Card,
  },
};
</script>

<template>
  <main>
    <div class="center main-one-bg">
      <div class="container pt-24 pb-24 relative">
        <div class="absolute">
          <button
            class="white ps-16 pt-8 pb-8 pe-16 with-cursor-pointer main-two-bg no-border"
          >
            CURRENT SERIES
          </button>
        </div>
        <div class="d-flex wrap">
          <Card
            v-for="(card, i) in cards"
            :key="i"
            :product="card"
            class="width-a-sixth white margin-trentadue"
          />
        </div>
        <div class="center">
          <button
            class="white ps-16 pt-8 pb-8 pe-16 with-cursor-pointer main-two-bg no-border"
          >
            LOAD MORE
          </button>
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
.relative {
  position: relative;
}
.absolute {
  position: absolute;
  top: calc(-31.5px / 2);
}
</style>
