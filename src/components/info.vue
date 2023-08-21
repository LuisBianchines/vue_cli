<template>
  <div>
    <p v-if="trabalhando">Estou trabalhando no momento</p>
    <p v-else>Buscando novas oportunidades</p>
    <p v-if="4 > 6">Maior</p>
    <p v-else>menor</p>
    <p>Tecnologias Backend:</p>
    <ul>
      <li v-bind:key="index" v-for="(stack, index) in backend">{{ stack }}</li>
    </ul>
    <p>Tecnologias Frontend:</p>
    <ul>
      <li v-for="stack in frontend" :key="stack.id">
        {{ stack.language }}
      </li>
    </ul>

    <div>
      <button @click="ShowEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Enviar email para {{ email }}</p>

    <p>Para acessar meu portfólio <a v-bind:href="meu_link">Clique Aqui</a></p>
    <Picture />

    <p>Utilizo as seguintes linguagens:</p>
    <ul>
      <li>Delphi</li>
      <li>JavaScript</li>
    </ul>
    <p>E os seguintes Frameworks</p>
    <ul>
      <li>Vue.js</li>
      <li>Horse</li>
    </ul>
  </div>
</template>

<script>
    import Picture from './Picture.vue';
    export default {
        name : 'InfoPessoa',
        components: {
            Picture
        },
        data(){
            return {
                trabalhando: false,
                email: 'luishdb@hotmail.com',
                mostrar_email: true,
                meu_link: 'http://google.com',
                textoBotao: 'Mostrar E-mail',
                backend: ["JavaScript","PHP","Python","Delphi"],
                frontend: [
                    {id: 1, language: "Vue"},
                    {id: 2, language: "React"},
                    {id: 3, language: "Angular"}
                ]                
            }
        },
        methods: {
            ShowEmail(){
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email){
                    this.textoBotao = 'Mostrar E-mail'
                }else{
                    this.textoBotao = 'Esconder E-mail'
                }
            }
        }
    }
</script>