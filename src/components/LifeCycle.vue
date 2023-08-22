<template>
  <div>
    <h1>Qual sua Stack {{ valor }}</h1>
  </div>
</template>

<script>
export default {
  name: "LyfeCycle",
  data() {
    return {
      valor: "ainda nao sei",
    };
  },
  created() {
    setTimeout(() => {
      this.valor = "Backend";
    }, 1000);

    this.LifeCycle();
  },
  mounted() {
    setTimeout(() => {
      this.valor = "Frontend";
    }, 2000);

    this.LifeCycle();
  },
  methods: {
    LifeCycle() {
      //console.log('Deu certo');
    },
  },
};
</script>