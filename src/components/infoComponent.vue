<template>
    <div>
        <p>Estou trabalhando no momento</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
        <p>Meu perfil: <a v-bind:href="perfil_link" target="_blank">Clica</a></p>
        <profileComponent />
    </div>
</template>

<script>

    import profileComponent from './profile.vue';
    export default {
        name: 'InfoComponent',
        components: {
            profileComponent
        },
        data() {
            return {
                perfil_link: "https://www.google.com"
            }
        }
    }
</script>