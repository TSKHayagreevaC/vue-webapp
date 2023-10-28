<script setup>
import { ref, reactive } from 'vue'
  
// component logic
// declare some reactive state here.

  const counter = reactive({
    count: 0
  })
  
  console.log(counter.count)
  counter.count++
  
  const message = ref('Hello world')
  console.log(message.value)
  
  message.value="civic radar level madam"
  counter.count = message.value.split(' ').length

</script>

<template>
    <div>
        <h3>Declerative Rendering</h3>
        <h6>Words : {{message.split('').reverse().join("")}}</h6>
        <h6>Reverse : {{message.split('').reverse().join("")}}</h6>
        <p>Words Count : {{counter.count}}</p>
    </div>
</template>