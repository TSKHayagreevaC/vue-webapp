<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>

<template>
  <div>
    <h3>Event Listener</h3>
    <button v-on:click="increment">count is: {{ count }}</button>
  </div>
</template>