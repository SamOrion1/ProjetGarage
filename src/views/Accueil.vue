<template>
  <div class="Accueil">

    <v-main>
      
      <h1>Lorem, ipsum.</h1>
      <carousel />
      <h1>Lorem, ipsum.</h1>
      <card />

    </v-main>

</div>
</template>

<script>
import Carousel from '@/components/compAccueil/carousel.vue';
import Card from '@/components/compAccueil/card.vue'

  export default {
    name: 'Accueil-S',

    components: {
    Carousel,
    Card
},
  }
</script>

<style lang="scss">
.Accueil {
  // background-image: url('@/assets/bg.jpg');
  background-color: #424242;
}

h1{
  color: white;
  text-align: center;
  margin-top: 5%;
}

</style>