<template>
    <form @submit="enviarFormulario($event)" >
        <div>
            <InputText v-model="name" :value="name" />
        </div>
        <div>
            <InputText v-model="email" :value="email" />
        </div>
        <SubmitBtn />
    </form>
</template>

<script>
    import InputText from "./forms/InputText.vue";
    import SubmitBtn from "./forms/SubmitBtn.vue";

    export default {
        name: "FormPessoa",
        components: {
            InputText,
            SubmitBtn
        },
        data() {
            return({
                name: "Roberto",
                email: "robeto#liam.com"
            });
        },
        methods: {
            enviarFormulario(e) {
                e.preventDefault();
                
            }
        }
    };
</script>

<style scoped>
    form {
        margin-bottom: 110px;
        text-align: center;
        width: 13%;
    }
</style>