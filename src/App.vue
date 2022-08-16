<template>
  <div>
    <PrimeiroComponent />
    <p>Morada: {{ morada }}</p>
  </div>
</template>

<script>
  import PrimeiroComponent from './components/PrimeiroComponent.vue';


  export default {
    name: 'App',
    components: {
      PrimeiroComponent
    },
    data () {
      return {
        morada: 'Gamek'
      }
    }
  }
</script>