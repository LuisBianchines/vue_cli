<template>
  <div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Projetos</a></li>
      <li><a href="#">Contato</a></li>
      <li v-if="logado"><a href="#">Meu Perfil</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HeaderTeste",
  props: ["logado"]
};
</script>
 
 <style scoped>
div{
    text-align: center;

} 
ul {
  display: flex;  
  list-style: none;
  font-size: 20px;
  background-color: brown;
}

li {
  margin-left: 200px;
}

a {
  color: #ddd;
  text-decoration: none;
  transition: 0.5s;
}

a:hover {
  color: black;
}
</style>