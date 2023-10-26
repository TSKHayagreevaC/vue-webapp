<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <div>
    <h1>Event Listener: @click</h1>
    <button v-on:click="increment">count is: {{ count }}</button>
  </div>
</template>