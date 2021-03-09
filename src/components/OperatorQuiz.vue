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
  },
  methods: {
    startQuiz() {
      /* Quiz logik stegvis */
      /* 1. Slumpa två operander */
      /* 2. Beräkna korrekt svar */
      /* 3. Generera felaktiga svar */
      /* 4. Blanda svaren */
    }
  }
};
</script>

<style></style>
