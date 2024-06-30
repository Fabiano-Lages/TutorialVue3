<template>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades.</p>
    <p>Utilizo as seguintes tecnologias para o backend:</p>
    <ul>
        <li v-for="(tecnology, ind) in backend_tecnologies" :key="ind">{{ tecnology }}</li>
    </ul>
    <p>Utilizo as seguintes tecnologias para o frontend:</p>
    <ul>
        <li v-for="front in frontend_technologies" :key="front.id">{{ front.language }}</li>
    </ul>
    <div>
        <button @click="showEmail">Mostrar e-mail</button>
    </div>
    <p v-show="mostrar_email">Mandar uma mensagem para: {{ email }}</p>
    <p>Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
    <PicAvatar />
</template>

<script>
import PicAvatar from "./PicAvatar.vue"
    export default {
        name: "InfoPessoa",
        data() {
            return({
                esta_trabalhando: false,
                mostrar_email: false,
                email: "fabianolages@gmail.cvom",
                meu_link: "https://github.com/Fabiano-Lages",
                backend_tecnologies: [
                    "JavaScript", "PHP", "C#", "Python"
                ],
                frontend_technologies: [
                    {id: 1, language: "HTML" },
                    {id: 2, language: "CSS" },
                    {id: 3, language: "Vue" }
                ]
            });
        },
        computed: {
            tecnologiaGeral() {
                return([].concat(this.backend_tecnologies).concat(this.frontend_technologies));
            }
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email;
            }
        },
        components: {
            PicAvatar
        }
    };
</script>