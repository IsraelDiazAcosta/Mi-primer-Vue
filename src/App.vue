
<script setup>
const name="Hola parce";
const arrayFrutas = [
    {
        name: "Manzana",
        price: "$1.00",
        description: "Una manzana",
        stock: 0,
    },
    {
        name: "Pera",
        price: "$2.00",
        description: "Una pera",
        stock: 10,
    },
    {
        name: "Naranja",
        price: "$3.00",
        description: "Una naranja",
        stock: 20,
    },
];
      
</script>

<template>
  <h1> Hola {{ name .toUpperCase()}} </h1>

  <ul>
    <template v-for="furta in arrayFrutas" :key="furta.name">
      <li v-if="furta.stock > 0">
        {{ furta.name }} - {{ furta.price }} - {{ furta.stock }} 
      </li>

    </template>
  </ul>
  
  </template>

  <style>
  h1{
    color: brown;

  }

</style>
