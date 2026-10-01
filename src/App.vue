
<script setup>
const name="Hola parce";

const handleClick=(message)=>{
  console.log('message')
}
      
</script>

<template>
  <h1> Hola {{ name .toUpperCase()}} </h1>
  <button v-on:click="handleClick('me activaste')">Activame bro</button>
  <button @click="handleClick('me activaste')">Activame bro</button>

  
  </template>

  <style>
  h1{
    color: brown;

  }

</style>
