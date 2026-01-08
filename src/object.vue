<script setup>
import { reactive } from 'vue'

const user1 = reactive({ name: '', age: 0 })
</script>

<template>
 <div>
    <input v-model="user1.name" placeholder="Name" />
    <input v-model="user1.age" type="number" placeholder="Age" />
    <p>Hello, {{ user1.name }}! You are {{ user1.age }} years old.</p>
  </div>
 
</template>

<style scoped></style>