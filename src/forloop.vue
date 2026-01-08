<script setup >

import {ref} from 'vue'

const task = ref([])
const newtask = ref('')

const addtask = () => 
{
if(newtask.value)
{
    task.value.push(newtask.value)
}
newtask.value = ''
}

</script>

<template>

<div>

<input v-model = "newtask" placeholder="enter your name ">
<button @click="addtask"> add </button>

<ul>

<li v-for="(task ,index) in task" key:index>
{{task}}
</li>

</ul>
</div>
</template>

<style scoped></style>


