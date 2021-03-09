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
      this.operandLeft = Math.floor(Math.random() * 13);
      this.operandRight = Math.floor(Math.random() * 13);

      if (this.operator == "+") {
        /* 2. Beräkna korrekt svar */
        this.expectedAnswer = this.operandLeft + this.operandRight;

        /* 3. Generera felaktiga svar */
      }

      /* 4. Blanda svaren */
    }
  },
  created() {
    this.startQuiz();
  }
};
</script>

<style></style>
