<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Nome: {{ nome }}</p>
        <p>Profissão: {{ profissao }}</p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponent',
        data () {
            return {
                nome: 'Nehrú',
                profissao: 'Programador'
            }
        }
    }
</script>