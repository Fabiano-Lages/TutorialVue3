<template>
    <form action="">
        <div>
            <InputText />
        </div>
        <div>
            <InputText />
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
        }
    };
</script>