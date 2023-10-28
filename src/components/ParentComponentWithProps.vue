<script setup>
    import {ref} from 'vue';
    import ChildComponentWithProps from './childComponents/ChildComponentWithProps.vue';
    const greeting = ref('Hello from Parent..!');
</script>

<template>
    <div>
        <h3>Parent Component With Props</h3>
        <ChildComponentWithProps :msg="greeting" />
    </div>
</template>