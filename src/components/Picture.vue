<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default {
        name: 'PictureTeste',
        data(){
            return{
                avatar: "/img/avatar.png",
                descricao: "Teste"
            }
        }
    } 
</script>