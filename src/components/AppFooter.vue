<script>
export default {
  data() {
    return {
      dc_comics: [
        {
          link: "Characters",
        },
        {
          link: "Comics",
        },
        {
          link: "Movies",
        },
        {
          link: "TV",
        },
        {
          link: "Games",
        },
        {
          link: "Videos",
        },
        {
          link: "News",
        },
      ],
      shop: [
        {
          link: "Shop DC",
        },
        {
          link: "Shop DC Collectibles",
        },
      ],
      dc: [
        {
          link: "Terms Of Use",
        },
        {
          link: "Privacy policy (New)",
        },
        {
          link: "Add Choices",
        },
        {
          link: "Advertising",
        },
        {
          link: "Jobs",
        },
        {
          link: "Subscriptions",
        },
        {
          link: "Talent workshops",
        },
        {
          link: "CPSC Certificates",
        },
        {
          link: "Ratings",
        },
        {
          link: "Shop Help",
        },
        {
          link: "Contact us",
        },
      ],
      sites: [
        {
          link: "DC",
        },
        {
          link: "MAD Magazine",
        },
        {
          link: "DC Kids",
        },
        {
          link: "DC Universe",
        },
        {
          link: "DC Power Visa",
        },
      ],
      social: [
        {
          img: "../../src/assets/img/footer-facebook.png",
        },
        {
          img: "../../src/assets/img/footer-twitter.png",
        },
        {
          img: "../../src/assets/img/footer-youtube.png",
        },
        {
          img: "../../src/assets/img/footer-pinterest.png",
        },
        {
          img: "../../src/assets/img/footer-periscope.png",
        },
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <footer>
    <div class="center footer-one-height footer-one-bg">
      <div class="h-100 container">
        <div class="h-100 d-flex">
          <div class="col-footer-width white pt-24 pb-24">
            <div class="mb-8">DC COMICS</div>
            <ul class="no-decoration mb-16">
              <li v-for="(link, i) in dc_comics" class="mb-2">
                <a class="no-underlining footer-grey smaller-plus" href="">{{
                  link.link
                }}</a>
              </li>
            </ul>
            <div class="mb-8">SHOP</div>
            <ul class="no-decoration">
              <li v-for="(link, i) in shop" class="mb-2">
                <a class="no-underlining footer-grey smaller-plus" href="">{{
                  link.link
                }}</a>
              </li>
            </ul>
          </div>
          <div class="col-footer-width white pt-24 pb-24">
            <div class="mb-8">DC</div>
            <ul class="no-decoration">
              <li v-for="(link, i) in dc" class="mb-2">
                <a class="no-underlining footer-grey smaller-plus" href="">{{
                  link.link
                }}</a>
              </li>
            </ul>
          </div>
          <div class="col-footer-width white pt-24 pb-24">
            <div class="mb-8">SITES</div>
            <ul class="no-decoration">
              <li v-for="(link, i) in sites" class="mb-2">
                <a class="no-underlining footer-grey smaller-plus" href="">{{
                  link.link
                }}</a>
              </li>
            </ul>
          </div>
          <div class="grow-one dc-logo-bg"></div>
        </div>
      </div>
    </div>

    <div class="center footer-two-height footer-two-bg">
      <div class="container h-100 spaced-centered-divs">
        <div class="h-100 centered-vertically-div">
          <div>
            <button
              class="border-botton-color footer-two-bg white with-cursor-pointer ps-8 pt-8 pb-8 pe-8"
            >
              SIGN-UP NOW!
            </button>
          </div>
        </div>
        <div class="h-100 centered-vertically-div">
          <div class="footer-blu ps-8 pe-8">FOLLOW US</div>
          <div v-for="(elemento, i) in social" class="ps-4 pe-4">
            <a href=""><img :src="elemento.img" alt="" /></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/mixins.scss" as *;
.footer-one-height {
  height: $footer_one_height;
}
.footer-two-height {
  height: $footer_two_height;
}
.footer-two-bg {
  background-color: $footer_two_bg;
}
.footer-one-bg {
  background-image: url(../assets/img/footer-bg.jpg);
}
.col-footer-width {
  width: calc(100% / 5.8);
}
.border-botton-color {
  border: 3px solid $footer_blu;
}
.h-100px {
  height: 100px;
}
.dc-logo-bg {
  background-image: url("../assets/img/dc-logo-bg.png");
  background-size: cover;
  background-position: center;
}
</style>
