<script>
export default {
  data() {
    return {};
  },
  props: {
    product: Object,
  },
};
</script>

<template>
  <div class="single-card">
    <div>
      <img :src="product.thumb" :alt="product.series" class="w-100" />

      <h6>
        {{ product.series }}
      </h6>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/mixins.scss" as *;
</style>
