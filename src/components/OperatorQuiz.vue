<template>
  <div>
    <!-- Visa uttrycket genom att interpolera operanderna och operatorn -->
    <p>{{ operandLeft }} {{ operator }} {{ operandRight }}</p>
    <button @click="$emit('clearOperator')">Back</button>
  </div>
</template>

<script>
export default {
  name: "OperatorQuiz",
  props: ["operator"],
  data() {
    /* Variabler som används i quiz för att hålla koll på uttrycket,
    svarsalternativen och det korrekta svaret. */
    return {
      operandLeft: null,
      operandRight: null,
      answers: [],
      expectedAnswer: null
    };
  }
};
</script>

<style></style>
