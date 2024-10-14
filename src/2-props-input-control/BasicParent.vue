<script setup lang="ts">
import BasicInput from '@/2-props-input-control/BasicInput.vue'
import { ref, watch } from 'vue'

const userName = ref<string>('')
const password = ref<string>('')

watch(userName, () => {
  console.log(userName.value)
})
</script>

<template>
  <BasicInput v-model:user-name="userName" v-model:password="password" form-title="Registration" />

  <div>Hacker watching</div>
  <div>Username is {{ userName }}</div>
  <div>Password is {{ password }}</div>
</template>

<style scoped></style>
