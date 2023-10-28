<script setup>
import { ref } from 'vue'

const titleClass = ref('title')
const descriptionClass = ref('description')
</script>

<template>
  <div>
    <h3 :class="titleClass">Title</h3> 
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