<template>
  <div>
    <h3>{{ foo }}, {{ bar }}</h3>
  </div>
</template>

<script setup lang="ts">
defineProps<{ foo: string, bar: string }>()
</script>
