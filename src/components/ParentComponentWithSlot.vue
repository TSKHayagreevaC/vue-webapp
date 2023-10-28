<script setup>
    import {ref} from 'vue';
    import ChildComponentWithSlot from './childComponents/ChildComponentWithSlot.vue';

    const msg = ref('This is some slot content from Parent Component!');
</script>

<template>
    <div>
        <h3>Parent Component With Slot</h3>
        <ChildComponentWithSlot>Message :: {{msg}}</ChildComponentWithSlot>
    </div>
</template>