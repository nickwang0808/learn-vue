<script setup lang="ts">
import { ref, watch } from 'vue'

const count = ref<number>(0)

function changeCountBy(changeBy: number) {
  count.value += changeBy
}

watch([count], (prev) => {
  console.log(`prevcount is ${prev}`)
  console.log(`new count is ${count.value}`)
})
</script>

<template>
  <div>Counter: {{ count }}</div>

  <button @click="count++">Increment</button>
  <button @click="count--">Decrement</button>

  <button @click="changeCountBy(5)">Add 5</button>
  <button @click="changeCountBy(-3)">Remove 3</button>
</template>

<style scoped></style>
