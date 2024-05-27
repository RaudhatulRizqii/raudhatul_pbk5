<template>
  <div class="q-pa-md">
    <q-layout view="lHh lpr lFf"  class="shadow-2 rounded-borders">
      <q-header elevated>
        <q-toolbar class="glossy">
          <q-btn flat round dense icon="menu" class="q-mr-sm" />
          <q-avatar>
            <img src="./assets/mac.jpg">
          </q-avatar>

          <q-toolbar-title>Raudhatu Laptop</q-toolbar-title>

        </q-toolbar>
      </q-header>

      

      <q-page-container>
        <q-card class="my-card">
      <img src="./assets/mac.jpg">

      <q-card-section>
        <div class="text-h6">Price 22.0000.000</div>
        <div class="text-subtitle2">Laptop mac</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        {{ lorem }}
      </q-card-section>
    </q-card>
    <q-carousel
        v-model="slide"
        transition-prev="scale"
        transition-next="scale"
        swipeable
        animated
        control-color="white"
        navigation
        padding
        arrows
        height="300px"
        class="bg-primary text-white shadow-1 rounded-borders"
      >
        <q-carousel-slide name="style" class="column no-wrap flex-center">
          <q-icon name="style" size="56px" />
          <div class="q-mt-md text-center">
            <img src="./assets/acer.jpg">
          </div>
        </q-carousel-slide>
        <q-carousel-slide name="tv" class="column no-wrap flex-center">
          <q-icon name="live_tv" size="56px" />
          <div class="q-mt-md text-center">
            <img src="./assets/mac.jpg">
          </div>
        </q-carousel-slide>
        <q-carousel-slide name="layers" class="column no-wrap flex-center">
          <q-icon name="layers" size="56px" />
          <div class="q-mt-md text-center">
            <img src="./assets/tuf.jpg">
          </div>
        </q-carousel-slide>
        <q-carousel-slide name="map" class="column no-wrap flex-center">
          <q-icon name="terrain" size="56px" />
          <div class="q-mt-md text-center">
          </div>
        </q-carousel-slide>
      </q-carousel>
      </q-page-container>
      <q-footer elevated>
        <q-toolbar class="glossy">
          <q-toolbar-title>Footer</q-toolbar-title>
        </q-toolbar>
      </q-footer>
    </q-layout>
  </div>
</template>

  
 
      
<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('style'),
      lorem: 'Pre-Order 1-6 days'
    }
  }
}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px
</style>