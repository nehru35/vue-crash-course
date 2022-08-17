<template>
    <img :src="avatar" :alt="descricao">

</template>

<script>
    export default {
        name: 'profileComponent',
        data() {
            return {
                avatar: '/img/perfil.png',
                descricao: 'Matheus André'
            }
        }
    }
</script>