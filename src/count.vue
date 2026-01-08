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
const no = ref (0)

const increase = () => no.value++
const decrease = () => no.value--

</script>

<template>
  <h1>You did it!</h1>
  <p>
   {{message}}
  </p>
  <button @click="ChangeWord" > next</button>
<button @click="BackWord"  > back</button>

  <p>
   {{no}}
  </p>
  <button @click="increase" > +</button>
<button @click="decrease"  >-</button>



</template>

<style scoped></style>
