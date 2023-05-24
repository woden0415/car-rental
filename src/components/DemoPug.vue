<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)
const addCount = () => {
  count.value += 1
}
const reduceCount = () => {
  count.value -= 1
}
</script>

<template lang="pug">
div.red-color() {{ count  }}
button(@click="addCount") addCount
button(@click="reduceCount") reduceCount
</template>

<style scoped>
</style>
