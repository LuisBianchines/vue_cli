<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ valor }}</h2>
        <Info compEmail="luis@teste.com.br" :email="email" :trabalhando="true"/>
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
            valor: 'Luis',
            email: 'testeemailprops@teste.com'
        };
    },
    components: {
    Info,
    Form
}
}
   
</script>