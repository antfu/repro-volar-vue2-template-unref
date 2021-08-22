<template>
  <div>
    <hello-world
      :foo="a"
      :bar="b"
     />
  </div>
</template>

<script setup lang="ts">
import HelloWorld from './HelloWorld.vue'
import { ref } from '@vue/composition-api'

const a = ref('Hi')
const b = ref('Hello')
</script>
