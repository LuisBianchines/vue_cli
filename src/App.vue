<template>
  <div>
    <PrimeiroComponente/>,
    <p>isso também é um componente mesmo sendo o root</p>
    
  </div>
  
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';

export default {
  name : 'App',
  components: {
    PrimeiroComponente
  },
  data() {
    return {
      teste: "teste"
    }
  }

}
</script>