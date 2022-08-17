<template>
  <div>
    <PrimeiroComponent />
    <LifeCycle />
    <p>Morada: {{ morada }}</p>

    <PessoaComponent />
    <FormComponent />
  </div>
</template>

<script>
  import PrimeiroComponent from './components/PrimeiroComponent.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import PessoaComponent from './components/PessoaComponent.vue';
  import formComponent from './components/formComponent.vue';



  export default {
    name: 'App',
    components: {
    PrimeiroComponent,
    LifeCycle,
    PessoaComponent,
    formComponent
},
    data () {
      return {
        morada: 'Gamek'
      }
    }
  }
</script>