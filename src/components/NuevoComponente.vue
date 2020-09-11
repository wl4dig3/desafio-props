<template>
<div>
    <h1>{{message1}}</h1>
    <form action="">
        <input type="text" placeholder="Add To list">
        <button>+</button>
    </form>
</div>
</template>

<script>
export default {
    name: 'NuevoComponente',
    props: {
        msssg: String
    },
    data() {
        return {
            message1: 'soy el nuevo componente en NUevo Componente '
        }
    }
}
</script>
