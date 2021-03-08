<template>
  <button @click="$emit('changeOperator', '+')">
    Addition +
  </button>
  <button @click="$emit('changeOperator', '-')">
    Subtraktion -
  </button>
  <button @click="$emit('changeOperator', '/')">
    Division /
  </button>
  <button @click="$emit('changeOperator', '*')">
    Multiplikation *
  </button>
</template>

<script>
export default {
  name: "OperatorSelector"
};
</script>

<style></style>
