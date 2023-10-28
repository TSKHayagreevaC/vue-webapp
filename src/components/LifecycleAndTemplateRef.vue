<script setup>
    import {ref, onMounted} from 'vue';
    const paraElementRef = ref(null);

    onMounted(() => {
        paraElementRef.value.textContent = "Mounted..!"
    })

</script>

<template>
    <div>
        <p ref="paraElementRef">Hello</p>
    </div>
</template>