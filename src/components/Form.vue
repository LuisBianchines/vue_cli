<template>
  <div>
    <h2>Meu formulário</h2>
    <form action="" @submit="enviarFormulario($event)">
      <div>
        <InputText />
      </div>
      <div>
        <InputText />
      </div>
      <div>
        <input type="text" v-model="name" />
      </div>
      <div>
        <input type="text" v-model="email" />
      </div>
      <div>
        <Submit />
      </div>
    </form>
  </div>
</template>

<script>
import InputText from "./form/InputText.vue";
import Submit from "./form/Submit.vue";

export default {
  name: "FormInputs",
  components: {
    InputText,
    Submit,
  },
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("Formulário enviado");
      console.log("o nome é " + name);
      console.log("o email é " + email);
    },
  },
};
</script>

<style scoped>
div {
  background-color: brown;
  text-align: center;
  margin-bottom: 5px;
}
</style>