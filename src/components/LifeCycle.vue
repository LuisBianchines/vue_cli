<template>
    <div>
        <h1>o valor é {{ valor }}</h1>
    </div>
    
</template>

<script>
    export default {
        name: 'LyfeCycle',
        data(){
            return {
                valor: 'ainda nao sei'
            }
        },
        created(){
            setTimeout(() => {
                this.valor = '9000'    
            }, 1000);   
            
            this.LifeCycle()
        },
        mounted(){
            setTimeout(() => {
                this.valor = '2000'    
            }, 2000);

            this.LifeCycle()
            
        },
        methods: {
            LifeCycle(){
                console.log('Deu certo');
            }
        }
    }
</script>