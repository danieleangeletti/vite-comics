<script>
export default {
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <footer>
    <div class="center footer-one-height footer-one-bg">
      <div class="container">
        <div>FOOTER 1</div>
      </div>
    </div>

    <div class="center footer-two-height footer-two-bg">
      <div class="container">
        <div>FOOTER 2</div>
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
</style>
