<template>
  <div class="Services">

    <v-main>
      
      <tableauPrestation />
    </v-main>
    
</div>
</template>

<script>
  import tableauPrestation from '@/components/compServices.vue/tableauPrestation.vue';

  export default {
    name: 'Services-S',

    components: {
      tableauPrestation,
    },
  }
</script>

<style lang="scss">
 
</style>