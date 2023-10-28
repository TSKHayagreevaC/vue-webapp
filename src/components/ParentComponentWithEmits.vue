<script setup>
    import {ref} from 'vue';
    import ChildComponentWithEmits from './childComponents/ChildComponentWithEmits.vue';
    const childMsg = ref('No Child Message Yet');
</script>

<template>
    <div>
        <h3>Parent Component With Emits</h3>
        <ChildComponentWithEmits @response="(msg) => childMsg = msg" />
        <p>{{childMsg}}</p>
    </div>
</template>