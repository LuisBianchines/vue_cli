<template>
  <div>
    <Header />
    <MultiplosEventos />
    <PrimeiroComponente/>
    <LifeCycle/>
    <Pessoa/>
    
  </div>
  
</template>

<script>
import Header from './components/Header.vue';
import MultiplosEventos from './components/MultiplosEventos.vue';
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';


export default {
  name : 'App',
  components: {
    Header,
    MultiplosEventos,
    PrimeiroComponente,
    LifeCycle,
    Pessoa

},
  data() {
    return {
      teste: "teste"
    }
  }

}
</script>

<style>
   body {
     background-color: #333;
     color: #fff;
   }

   a {
     color: dodgerblue;
     /*font-size: 30px;*/
     font-style: italic;
   }
</style>