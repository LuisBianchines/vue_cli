<template>
  <button @click="primeiro(txt1), segundo(txt2), terceiro(txt3)">
    Mostrar Multiplos Eventos
  </button>
  <p>{{ Multiplos_Eventos }}</p>
</template>

<script>
export default {
  name: "MostarMultiplosEventos",
  data() {
    return {
      Multiplos_Eventos: "",
      txt1: "Primeiro Evento",
      txt2: "Segundo Evento",
      txt3: ""
    };
  },
  methods: {
    primeiro(txt) {
      this.Multiplos_Eventos = txt;
    },
    segundo(txt) {
      setTimeout(() => (this.Multiplos_Eventos = txt), 1000);

    },
    terceiro(txt){
        setTimeout(() => (this.Multiplos_Eventos = txt), 2000);
    }
  },
};
</script>