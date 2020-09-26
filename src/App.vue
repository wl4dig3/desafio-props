<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />

    <NuevoComponente :msssg="Nuevo" @accion="sustract"/>

    <ComponentHijo :mensajito="mensajito2" />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import NuevoComponente from "./components/NuevoComponente.vue";
// import ComponentHijo from "./components/ComponentHijo.vue";

export default {
  name: "App",
  components: {
    NuevoComponente,
    // ComponentHijo,
  },
  data() {
    return {
      mensajito2: "mensajito2 desde data",
      Nuevo: "Nueva props en el desafio ",
    };
  },
};
</script>
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
