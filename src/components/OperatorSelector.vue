<template>
  <button @click="$parent.operator = '+'">
    Addition +
  </button>
  <button @click="$parent.operator = '-'">
    Subtraktion -
  </button>
  <button @click="$parent.operator = '/'">
    Division /
  </button>
  <button @click="$parent.operator = '*'">
    Multiplikation *
  </button>
</template>

<script>
export default {
  name: "OperatorSelector"
};
</script>

<style></style>
