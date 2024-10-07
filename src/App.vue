<script setup lang="ts">
import { ref } from 'vue'

const counter = ref(0)

function increment(count: number) {
  counter.value += count
}

function decrement() {
  counter.value--
}

</script>

<template>
  <div>Count {{ counter }}</div>

  <button @click="() => increment(3)">Increment</button>
  <button @click="decrement">Decrement</button>
</template>

<style scoped></style>
