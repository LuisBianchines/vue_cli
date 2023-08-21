<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
    </ul>
</template>

<script>
   export default {
    name: 'HeaderTeste'
   }
 </script>
 
 <style scooped>
   ul {
      list-style: none;
      display: flex;
      font-size: 15px ;
   }

   li {
      margin-left: 10px;
   }
</style>