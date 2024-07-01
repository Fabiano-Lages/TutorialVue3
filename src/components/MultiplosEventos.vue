<template>
    <div>
        <button @click="primeiro('Primeiro evento!'),segundo('Segundo evento!'),terceiro('Terceiro evento!')">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>
<script>
    export default {
        name: "MultiplosEventos",
        data() {
            return({
                multiplos_eventos: ""
            })
        },
        methods: {
            primeiro(texto) {
                this.multiplos_eventos = texto;
            },
            segundo(texto) {
                setTimeout(() => this.multiplos_eventos = texto, 1000);
            },
            terceiro(texto) {
                setTimeout(() => this.multiplos_eventos = texto, 2000);
            }
        }
    }
</script>
<style scoped>
</style>