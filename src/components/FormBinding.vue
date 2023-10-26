<script setup>
import {ref} from 'vue'

const text = ref('')

function onInput(e) {
    text.value = e.target.value
}

</script>

<template>
    <div>
        <input :value="text" @input="onInput" placeHolder="Enter Text Here">
        <p>{{text}}</p>
    </div>
</template>

<style scoped>
</style>