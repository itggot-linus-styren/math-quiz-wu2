<template>
  <button @click="operator = '+'">
    Addition +
  </button>
  <button @click="operator = '-'">
    Subtraktion -
  </button>
  <button @click="operator = '/'">
    Division /
  </button>
  <button @click="operator = '*'">
    Multiplikation *
  </button>
</template>

<script>
export default {
  name: "OperatorSelector",
  data() {
    return {
      operator: null
    };
  }
};
</script>

<style></style>
