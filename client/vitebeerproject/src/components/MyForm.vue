<template>
  <div>
    <p>{{ name }}</p>
    <input type="text" placeholder="Name" v-model="name" />
  </div>
  <button @click="submitForm">Submit v-bind:disabled="name.length==0"</button>
</template>

<script>
import {ref } from 'vue'

export defaul {
setup () {
const name = ref('')
const submitForm = () => {
console.log(`form submited name = ${name.value}`)

}
return {
name,
}

  },
}
</script>

<style>
input[type="text"] {
  padding: 5px;
}
button {
  margin-top: 20px;
}
</style>
