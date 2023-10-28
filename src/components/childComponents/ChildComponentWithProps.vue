<script setup>

    const props = defineProps({
        msg: String
    })

</script>

<template>
    <h1>Child Component With Props</h1>
    <p>{{ msg || 'No Props Passed Yet' }}</p>
</template>