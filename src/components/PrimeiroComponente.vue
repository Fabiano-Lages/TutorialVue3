<template>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{  nome  }} e trabalho como {{ profissao }}</p>
    <MultiplosEventos />
    <ReUtilizacao />
    <ReUtilizacao />
    <ReUtilizacao />
    <ReUtilizacao />
    <ReUtilizacao />
    <ReUtilizacao />
    <ReUtilizacao />
    <ReUtilizacao />
</template>

<script>
    import MultiplosEventos from "./MultiplosEventos.vue";
    import ReUtilizacao from "./ReUtilizacao.vue";
    
    export default {
        name: "PrimeiroComponernte",
        data() {
            return({
                nome: "Fabiano",
                profissao: "Analista de Sistemas"
            });
        },
        components: {
            MultiplosEventos,
            ReUtilizacao
        }
    }
</script>