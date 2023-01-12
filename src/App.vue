<template>
  <input type="text" v-bind:disabled="controlador" />
  <input type="text" :disabled="controlador" />
  <button @click="ativador">ativador</button>
</template>

<script>
export default {
  data() {
    return {
      controlador: true,
    };
  },
  methods: {
    ativador() {
      this.controlador = !this.controlador;
    },
  },
};
</script>

<style>
</style>
