<template>
    <div>
        <p v-if="trabalhando">Estou trabalhando no momento</p>
        <p v-else>Buscando novas oportunidades</p>
        <p v-if="4 > 6">Maior</p>
        <p v-else>menor</p>   

        <p v-show="mostrar_email">Enviar email para {{ email }}</p>
        
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
    export default {
        name : 'InfoPessoa',
        data(){
            return {
                trabalhando: false,
                email: 'luishdb@hotmail.com',
                mostrar_email: false
            }
        }
    }
</script>