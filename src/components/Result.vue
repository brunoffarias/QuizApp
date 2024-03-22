<script setup>
import { defineProps } from "vue";
const { numberOfCorrectAnswers, quizQuestionLength } = defineProps([
  "numberOfCorrectAnswers",
  "quizQuestionLength",
]);
</script>
<template>
  <div class="results"></div>
  <p>Your results...</p>
  <h1>{{ numberOfCorrectAnswers }}|{{ quizQuestionLength }}</h1>
</template>

<style scoped>
.results {
  text-align: center;
  padding: 100px 0;
}
p {
  font-size: 25px;
}

h1 {
  font-size: 80px;
}
</style>
