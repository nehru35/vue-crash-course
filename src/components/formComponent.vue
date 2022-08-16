<template>

    <form action="">
        <InputTextComponent />
        <InputTextComponent />
        <InputSubmitComponent />
    </form>

</template>

<script>
    import InputTextComponent from './form/inputText.vue';
    import InputSubmitComponent from './form/inputSubmit.vue';

    export default {
        name: 'FormComponent',
        components: {
            InputTextComponent,
            InputSubmitComponent
        }
    }
</script>