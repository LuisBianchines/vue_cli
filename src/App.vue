<template>
  <div>
    <PrimeiroComponente/>,
    <p>isso também é um componente mesmo sendo o root</p>,
    <LifeCycle/>
    
  </div>
  
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';

export default {
  name : 'App',
  components: {
    PrimeiroComponente,
    LifeCycle
  },
  data() {
    return {
      teste: "teste"
    }
  }

}
</script>