<template>
  <div>
    <p>{{ operator }}</p>
    <button @click="$emit('clearOperator')">Back</button>
  </div>
</template>

<script>
export default {
  name: "OperatorQuiz",
  props: ["operator"]
};
</script>

<style></style>
