<script setup lang="ts">
import { ref, watch } from 'vue'

const name = ref('')

const weirdName = ref('')

watch(name, (newName) => {
  weirdName.value = '-' + newName + '-'
})
</script>

<template>
  <div>{{ name }}</div>

  <input :value="name" @input.prevent="(e) => (name = e.target.value)" />
  <div>othername {{ weirdName }}</div>
</template>

<style scoped></style>
