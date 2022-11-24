<template>
  <div class="page">
    <div class="block"></div>
    <LazyImage
      src="/images/prague-conference-center-1056491.jpg"
      alt="Static image"
    />
    <LazyImage
      src="https://images.freeimages.com/images/large-previews/218/my-dog-cutter-1499799.jpg"
      alt="Free image"
    />
  </div>
</template>

<script>
  export default {
    name: 'IndexPage',
    components: {
      LazyImage: () => import('@/components/LazyImage')
    }
  }
</script>

<style>
  .page {

  }

  .block {
    height: 110vh;
  }
</style>
