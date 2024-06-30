<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name: "LifeCycle",
        data() {
            return({
                nome: "Ainda não sei"
            });
        },
        mounted() {
            setTimeout(() => {
                this.nome = "Cristina";
            }, 2000);

            this.lifeCycle("montado");
        },
        created() {
            setTimeout(() => {
                this.nome = "Fabiano";
            }, 1000);

            this.lifeCycle("criado");
        },
        methods: {
            lifeCycle(texto) {
                console.log("Executou " + texto)
            }
        }
    }
</script>