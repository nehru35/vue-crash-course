<template>
    <div>
        <p>Estou trabalhando no momento</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>

        <div>
            <button @click="mostarEmail"> {{ textoBotao }}</button>
        </div>
        <p v-show="mostrar">techn3hru@gmail.com</p>
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
                perfil_link: "https://www.google.com",
                mostrar : false,
                textoBotao: 'Mostrar Email'
            }
        },
        methods: {
            mostarEmail() {
                this.mostrar = !this.mostrar;
                if (!this.mostar) {
                    this.textoBotao = "Mostrar Email"
                } else {
                    this.textoBotao = "Esconder Email"

                }
            }
        }
    }
</script>