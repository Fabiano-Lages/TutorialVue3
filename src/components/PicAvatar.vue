<template>
    <img :src="avatar" :alt="descricao" width="200" />
</template>
<script>
    export default {
        name: "PicAvatar",
        data() {
            return({
                avatar: "/img/avatar.png",
                descricao: "Fabiano Teixeira Lages"
            });
        }
    }
</script>