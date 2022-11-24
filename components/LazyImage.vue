<template>
  <div class="lazy-image">
    <img
      :src="$img(src, { quality: 10, height: 100 })"
      v-lazy="{ src: src, loading: $img(src, { quality: 10, height: 100 }) }"
      :alt="alt"
    >
  </div>
</template>

<script>
  export default {
    name: "LazyImage",
    props: {
      src: {
        type: String,
        default: ''
      },
      alt: {
        type: String,
        default: ''
      }
    }
  }
</script>

<style scoped>
  .lazy-image img {
    width: 100%;
  }
</style>
