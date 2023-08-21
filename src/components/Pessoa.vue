<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ valor }}</h2>
        <Info />
        <Form />
    </div>
</template>

<script>
    import Info from './info.vue';
    import Form from './Form.vue';

    export default {
    name: 'PessoaTeste',
    data() {
        return {
            valor: 'Luis'
        };
    },
    components: {
    Info,
    Form
}
}
   
</script>