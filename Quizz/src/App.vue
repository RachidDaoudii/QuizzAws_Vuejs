<script setup>
import Stepper from './components/stepper.vue'
import StartQuizz from './components/StartQuizz.vue'
import ResultQuizz from './components/ResultQuizz.vue'
import info from './components/info.vue'
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <Stepper :callback="increment" :stp="count"/>
  <info :callback="increment" v-if="count == 0"  />
  <StartQuizz :callback="increment" v-if="count == 1" :stp="count" />
  <ResultQuizz v-if="count == 2" />
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
