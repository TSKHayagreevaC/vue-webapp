<script setup>
    import {ref, watch} from 'vue';

    const todoId = ref(1);
    const todoData = ref(null);

    async function fetchData () {
        todoData.value = null;
        const res = await fetch(
            `https://jsonplaceholder.typicode.com/todos/${todoId.value}`
        );
        todoData.value = await res.json();
    }

    fetchData();
    watch(todoId, fetchData);
</script>

<template>
    <div>
        <h3>Watchers</h3>
        <p>Todo Id: {{ todoId }}</p>
        <button @click="todoId++">Fetch Next Todo</button>
        <p v-if="!todoData">Loading...</p>
        <pre v-else>{{ todoData }}</pre>
    </div>
</template>
