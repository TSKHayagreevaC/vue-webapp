<script setup>
import { ref, computed } from 'vue'

let id = 0;

const newTodo = ref('');

const hideCompleted = ref(false);

const todos = ref([
    {id: id++,  text: 'Learn HTML', done: true},
    {id: id++, text: 'Learn Java Script', done: false},
    {id: id++, text: 'Learn Vue', done: true},
]);

function addTodo () {
    todos.value.push({id: id++, text: newTodo.value, done: false});
    newTodo.value = '';
}

function removeTodo (todo) {
    todos.value = todos.value.filter((t) => t !== todo)
}

const filteredTodos = computed(() => {
    return hideCompleted.value
        ? todos.value.filter((t) => !t.done)
        : todos.value
})

</script>

<template>
    <div>
        <h3>Computed Property</h3>
        <form @submit.prevent="addTodo">
            <input v-model="newTodo" >
            <button>Add Todo</button>
        </form>

        <ul>
            <li v-for="todo in filteredTodos" :key="todo.id">
                <input type="checkbox" v-model="todo.done" >
                <span :class="{done: todo.done}">{{todo.text}}</span>
                <button @click="removeTodo(todo)" >X</button>
            </li>
        </ul>
        <button @click="hideCompleted = !hideCompleted">
            {{hideCompleted ? 'Show All' : 'Hide Completed'}}
        </button>
    </div>
</template>

<style>
.done {
    text-decoration: line-through
}
</style>