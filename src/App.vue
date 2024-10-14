<script setup lang="ts">
import BasicState from '@/1-state-and-effects/BasicState.vue'
import BasicParent from '@/2-props-input-control/BasicParent.vue'
import ScrtchPad from '@/2-props-input-control/ScrtchPad.vue'
</script>

<template>
  <h3>1.</h3>
  <BasicState />

  <h3>2.</h3>
  <ScrtchPad />
  <basic-parent />
</template>

<style scoped></style>
