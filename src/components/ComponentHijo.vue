<template>
  <div>
      <b-button variant="danger" class="m-1" @click="accion">Sustract2</b-button>
    <h2>{{ mensajito }}</h2>
    <h3>Hola</h3>
  </div>
</template>

<script>
export default {
  name: "ComponentHijo",
  props: {
    mensajito: String,
  },
  methods: {
      accion(){
          this.$emit('accion')
      }
  },
};
</script>