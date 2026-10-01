
<script setup>
import { ref } from 'vue';
const name="Hola parce";

const counter=ref(0);
const increment=()=>{
  counter.value++;
}  

const disminuir=() =>{
  counter.value--;
}
const reset=() =>{
  counter.value =0;
}
</script>

<template>
  <h2  :style="{color:counter<0 ? 'red':counter>0 ? 'green': 'black'}">
    {{ counter }}
  </h2>
  <button @click="increment">Aumentar el contador</button>
  <button @click="disminuir">Disminuye el contador</button>
  <button @click="reset">Resetea el contador</button>
 
 
  </template>

  <style>
  h1{
    color: brown;

  }

</style>
