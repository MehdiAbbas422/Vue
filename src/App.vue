<script setup lang="ts">

import {ref} from 'vue'

//Reactive Veriable

const message = ref("hello bhaiyo")

const ChangeWord = () =>
{
message.value = "Wah wah"
}

const BackWord =()=>
{
  message.value ="hello bhaiyo"
}

</script>

<template>
  <h1>You did it!</h1>
  <p>
   {{message}}
  </p>
  <button @click="ChangeWord" > next</button>
<button @click="BackWord" > back</button>
</template>

<style scoped></style>
