<script setup lang="ts">
import { ref } from 'vue'

const notes = ref('')
</script>

<template>
  <textarea v-model="notes" />
</template>

<style scoped></style>
