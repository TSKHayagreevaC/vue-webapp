<script setup>
    import {ref, onMounted} from 'vue';
    const paraElementRef = ref(null);

    onMounted(() => {
        paraElementRef.value.textContent = "Mounted..!"
    })

</script>

<template>
    <div>
        <h3>Life Cycle & Template Ref</h3>
        <p ref="paraElementRef">Hello</p>
    </div>
</template>