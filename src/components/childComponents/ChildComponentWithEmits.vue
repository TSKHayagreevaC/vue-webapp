<script setup>
    const emit = defineEmits(['response']);
    emit('response', 'Hello from Child');
</script>

<template>
    <h3>Child Component With Emits</h3>
</template>