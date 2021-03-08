<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <h1>Math Quiz app</h1>
  <OperatorQuiz :operator="operator" />
  <OperatorSelector @changeOperator="onChangeOperator" />
</template>

<script>
import OperatorSelector from "./components/OperatorSelector.vue";
import OperatorQuiz from "./components/OperatorQuiz.vue";

export default {
  name: "App",
  data() {
    return {
      operator: null
    };
  },
  methods: {
    onChangeOperator(operator) {
      this.operator = operator;
    }
  },
  components: { OperatorSelector, OperatorQuiz }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

button {
  padding: 15px 32px;
}
</style>
