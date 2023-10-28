<script setup>
    const emit = defineEmits(['response']);
    emit('response', 'Hello from Child');
</script>

<template>
    <h1>Child Component With Emits</h1>
</template>