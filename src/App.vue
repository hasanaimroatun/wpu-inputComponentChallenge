<template>
  <InputComponents />
</template>

<script>
import InputComponents from"./components/InputComponents.vue";

export default {
  name: 'App',
  components: {
    InputComponents,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: '38px';
}
</style>
