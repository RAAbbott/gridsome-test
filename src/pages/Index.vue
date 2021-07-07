<template>
  <div class="w-full">
    <Banner/>
    <Grid class="my-36"/>
    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
  </div>
</template>

<script>
import Banner from '../components/Banner.vue'
import Grid from '../components/Grid.vue'
export default {
  components: {
    Banner,
    Grid
  },
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
</style>
