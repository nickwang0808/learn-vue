<script setup lang="ts">
import BasicState from '@/1-state-and-effects/BasicState.vue'
import BasicParent from '@/2-props-input-control/BasicParent.vue'
import ScratchPad from '@/2-props-input-control/ScratchPad.vue'
</script>

<template>
  <h3>1.</h3>
  <BasicState />

  <h3>2.</h3>
  <ScratchPad />
  <basic-parent />
</template>

<style scoped></style>
