<template>
    <input type="text" :value="value" />
</template>

<script>
    export default {
        name: "InputText",
        props: [
            'value' 
        ]
    };
</script>