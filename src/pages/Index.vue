<template>
  <div class="w-full">
    <Banner class="z-0"/>
    <Grid class="my-24"/>
    <Services/>
    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
  </div>
</template>

<script>
import Banner from '../components/Banner.vue'
import Grid from '../components/Grid.vue'
import Services from '../components/Services.vue'
export default {
  components: {
    Banner,
    Grid,
    Services
  },
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
</style>
