<template>
    <div>
       <button @click="reutilizar">Reutilizar</button>
       <span v-show="reutilizou">Reutilizou!</span>
    </div>
</template>

<script>
   export default {
    name: 'ReutilizacaoTeste',
    data(){
    return {
        reutilizou: false     
      }
     },
    methods: {
       reutilizar() {
         this.reutilizou = true
       }  
     }
   }
   

</script>