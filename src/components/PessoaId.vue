<template>
    <h3>{{ nome }}</h3>
    <InfoPessoa :email="email" :esta_trabalhando="false" />
    <FormPessoa />
</template>

<script lanf="ts">
    import InfoPessoa from "./InfoPessoa.vue";
    import FormPessoa from "./FormPessoa.vue";

    export default {
        name: "PessoaId",
        data() {
            return({
                nome: "Fabiano Teixeira Lages",
                email: "fabiano.lages@tenti.com.br"
            });
        },
        components: {
            InfoPessoa,
            FormPessoa
        }
    };
</script>