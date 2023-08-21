<template>
  <div>
    <Header />
    <PrimeiroComponente/>,
    <p>isso também é um componente mesmo sendo o root</p>,
    <LifeCycle/>,
    <Pessoa/>
    
  </div>
  
</template>

<script>
import Header from './components/Header.vue';
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

export default {
  name : 'App',
  components: {
    Header,
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