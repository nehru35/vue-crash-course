<template>
    <div>
        <h1>Nome: {{ name }}</h1>
    </div>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                name: 'Ainda não sei'
            }
        },
        created() {
            setTimeout(() => {
                this.name = "Matheus";
            }, 2000)
        },
        mounted() {
            setTimeout(() => {
                this.name = "Pedro"
            }, 5000)
        }
    }
</script>