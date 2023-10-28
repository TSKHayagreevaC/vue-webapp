<script setup>
    import {ref} from 'vue'
    const awesome = ref(true);
    function toggleText () {
        awesome.value = !awesome.value
    }
</script>

<template>
    <div>
        <h3 v-if="awesome">Awesome..!</h3>
        <h3 v-else="awesome">Oh No 😢</h3>
        <button @click="toggleText">Toggle Text</button>
    </div>
</template>