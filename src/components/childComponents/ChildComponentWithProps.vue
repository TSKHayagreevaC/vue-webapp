<script setup>

    const props = defineProps({
        msg: String
    })

</script>

<template>
    <h3>Child Component With Props</h3>
    <p>{{ msg || 'No Props Passed Yet' }}</p>
</template>