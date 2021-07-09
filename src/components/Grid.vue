<template>
<div class="text-center">
  <div class="text-4xl font-bold mb-12">Why Us?</div>
  <vue-glide>
    <vue-glide-slide v-for="item in items" :key="item.id">
      Slide {{item}}
    </vue-glide-slide>
  </vue-glide>
  <!-- <div class="flex flex-col xl:flex-row xl:justify-around justify-between 2xl:justify-center items-center">
      <div v-for="item in items" :key="item.id">
        <GridItem class="2xl:mx-12 mb-16" :data="item"/>
      </div>
  </div> -->

  <!-- Use tiny carousel instead! -->
</div>

</template>

<script>
import GridItem from './GridItem.vue'
import { Glide, GlideSlide } from 'vue-glide-js'
export default {
 components: {
   GridItem,
   [Glide.name]: Glide,
   [GlideSlide.name]: GlideSlide
 },

 data() {
   return {
     items: [
       {id: 1, icon: 'home', title: 'Experienced', text: 'We are a team of highly experienced and specialized individuals who make sure that every decision we make is qualified. From the research that goes into the design, to putting in the last nail, you can trust us through every step of the process.'},
       {id: 2, icon: 'recommend', title: 'Reliable', text: 'When it comes to reliability, we\'re number one. We\'re here to help you every step of the way, and we won\'t stop until you\'re satifsied. It\'s what we do!'},
       {id: 3, icon: 'handyman', title: 'Quality', text: 'The quality of our craftsmanship is unparalleled. We take immense pride in our work and will make sure every aspect of your home is exactly how you envisioned it.'},
     ]
   }
 }
}
</script>

<style>

</style>