<template>
  <div id="app">
    <BaseComponent msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import BaseComponent from "./components/BaseComponent.vue";

export default {
  name: "app",
  components: {
    BaseComponent
  }
};
</script>

<style>
@import "./assets/css/flexboxgrid.css";

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
