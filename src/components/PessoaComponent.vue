<template>
    <div>
        <h1>Está é a descrição da pessoa: {{ nome }}</h1>
        <InfoComponent />
    </div>
</template>

<script>
    import infoComponent from './infoComponent.vue';
import InfoComponent from './infoComponent.vue';

    export default {
        name: "PessoaComponet",
        components: {
    infoComponent,
    InfoComponent
},
        data() {
            return {
                nome: 'Matheus'
            }
        }
    }
</script>