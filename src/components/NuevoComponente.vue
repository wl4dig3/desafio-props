<template>
<div class="container">
    <h1 class="my-3">{{message1}}</h1>
    <form action>
        <b-form-input v-model="item" placeholder="Ingresa aqui una tarea nueva"></b-form-input>

    </form>
    <b-button variant="success" class="m-1" @click="add"> Add</b-button>

    <b-button variant="danger" class="m-1" @click="sustract"> Sustract</b-button>
    <ul v-for="item of items">
        <li>{{ item }}</li>
    </ul>
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
            items: [],
            item: '',
        };
    },
    methods: {

        add() {
            this.items.push(this.item);
            this.item = '';
        },
        sustract() {
            this.items.pop(this.item);
            this.item = '';

        },
    }
};
</script>

<style lang="scss" scoped>
ul {
    list-style: none;
    font-size: 1.2em;
}
</style>
