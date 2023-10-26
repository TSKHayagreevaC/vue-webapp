<script setup>
    import {ref} from 'vue'
    const awesome = ref(true);
    function toggleText () {
        awesome.value = !awesome.value
    }
</script>

<template>
    <div>
        <button @click="toggleText">Toggle Text</button>
        <h1 v-if="awesome">Awesome..!</h1>
        <h1 v-else="awesome">Oh no 😢</h1>
    </div>
</template>