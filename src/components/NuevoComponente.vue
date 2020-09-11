<template>
<div class="container">
    <h1 class="my-3">{{message1}}</h1>
    <form action>
        <b-form-input v-model="text" placeholder="Ingresa aqui una tarea nueva"></b-form-input>
        <div class="mt-2">Value: {{ texto }}</div>
    </form>
    <b-button variant="success" class="m-1">Add</b-button>
</div>
</template>

<script>
export default {
    name: "NuevoComponente",
    props: {
        msssg: String,
    },
    data() {
        return {
            message1: "Desafio de uso con props en Vue",

            texto: "aqui saldrá la la tarea",
        };
    },
};
</script>
