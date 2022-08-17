<template>
    <div>
        <h1>Está é a descrição da pessoa: {{ nome }}</h1>
        <infoComponent />

        <p v-if="mostra">Trabalhando...</p>
        <p v-else>Não trabalhando...</p>
        <p v-show="mostra">Trabalhando...</p>
    </div>
</template>

<script>
    import infoComponent from './infoComponent.vue';

    export default {
        name: "PessoaComponet",
        components: {
        infoComponent
    },
        data() {
            return {
                nome: 'Matheus',
                mostra: true
            }
        }
    }
</script>