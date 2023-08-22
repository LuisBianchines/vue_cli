<template>
  <img :src="avatar" :alt="descricao" />
  <MudarImagem @mudar-imagem="TrocarImagem"/>
</template>

<script>
import MudarImagem from './MudarImagem.vue';

export default {
    name: "PictureTeste",
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Teste",
        };
    },
    methods: {
        TrocarImagem() {
            this.avatar = "/img/avatar2.png"
        }
    },
    components: { MudarImagem }
};
</script>