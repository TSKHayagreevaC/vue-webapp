<script setup>
import { ref } from 'vue'

const titleClass = ref('title')
const descriptionClass = ref('description')
</script>

<template>
  <div>
    <h1 :class="titleClass">Title</h1> 
    <p :class="descriptionClass">Description...!</p>
  </div>
</template>

<style>
.title {
  color: green;
}
.description {
    color: grey;
}
</style>