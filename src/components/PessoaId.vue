<template>
    <h3>{{ nome }}</h3>
    <InfoPessoa />
    <FormPessoa />
</template>

<script lanf="ts">
    import InfoPessoa from "./InfoPessoa.vue";
    import FormPessoa from "./FormPessoa.vue";

    export default {
        name: "PessoaId",
        data() {
            return({
                nome: "Fabiano Teixeira Lages"
            });
        },
        components: {
            InfoPessoa,
            FormPessoa
        }
    };
</script>