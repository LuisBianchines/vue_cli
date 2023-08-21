<template>

  <div>
    <PrimeiroComponente/>,
    <p>isso também é um componente mesmo sendo o root</p>,
    <LifeCycle/>,
    <Pessoa/>
    
  </div>
  
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

export default {
  name : 'App',
  components: {
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

    <PrimeiroComponente/>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
 
  export default {
    name : 'App',
    components: {
      PrimeiroComponente
    }

  }

</script>