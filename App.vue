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
import type { Ref } from '@vue/runtime-dom'

const a = ref('Hi')

// assert to Vue3's ref it will work
const b = ref('Hello') as unknown as Ref<string>
</script>
