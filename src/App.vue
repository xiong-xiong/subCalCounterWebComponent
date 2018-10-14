<template>
  <div id="app">
      <Calculator 
      v-bind:breads="breads"
      v-bind:sauces="sauces" 
      v-bind:meats="meats"
      v-bind:cheeses="cheeses"  
      />
  </div>
</template>

<script>
import Calculator from "./components/Calculator.vue";
import { breads, sauces, meats, cheeses } from "./data/data.js";

export default {
  name: "app",
  components: {
    Calculator
  },
  data() {
    return {
      breads: breads,
      cheeses: cheeses,
      meats: meats,
      sauces: sauces
    };
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
