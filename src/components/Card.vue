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
      <div class="width-a-sixth height-a-sixth mb-16">
        <img :src="product.thumb" :alt="product.series" class="w-100 h-100" />
      </div>

      <h6 class="mb-32">
        {{ product.series }}
      </h6>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables.scss" as *;
@use "../assets/scss/partials/mixins.scss" as *;
</style>
