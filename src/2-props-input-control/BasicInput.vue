<script setup lang="ts">
defineProps({
  formTitle: {
    required: true,
    type: String
  },
  userName: {
    required: true,
    type: String
  },
  password: {
    required: true,
    type: String
  }
})

const emits = defineEmits(['update:userName', 'update:password'])

function handlePasswordUpdate(event: InputEvent) {
  emits('update:password', event.target.value)
}
</script>

<template>
  <div>{{ formTitle }}</div>
  <label>User name</label>
  <input :value="userName" @input="emits('update:userName', $event.target.value)" />

  <label>Password</label>
  <input :value="password" @input="handlePasswordUpdate" type="password" />
</template>

<style scoped></style>
