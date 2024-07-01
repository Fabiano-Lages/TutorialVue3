<template>
    <img :src="avatar" :alt="descricao" width="200" />
    <MudarImagem @mudarImagem="mudarImagem" />
</template>
<script>
    import MudarImagem from "./MudarImagem.vue";
    export default {
        name: "PicAvatar",
        data() {
            return({
                avatar: "/img/avatar.png",
                descricao: "Fabiano Teixeira Lages"
            });
        },
        components: {
            MudarImagem
        },
        methods: {
            mudarImagem() {
                this.avatar = this.avatar.indexOf("2") < 0 ? this.avatar.replace(".png", "2.png") : this.avatar.replace("2.png", ".png");
            }
        }
    }
</script>