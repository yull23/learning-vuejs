<script setup>
const arrayFruts = [
  {
    name: "Manzana",
    price: "$1.00",
    description: "Una manzana",
    count: 5,
  },
  {
    name: "Pera",
    price: "$2.00",
    description: "Una pera",
    count: 10,
  },
  {
    name: "Naranja",
    price: "$3.00",
    description: "Una naranja",
    count: 8,
  },
];
const number = 2

</script>
<template>
  <p>Hola</p>
  <ul v-for="(objectFruit, index) in arrayFruts" :key="objectFruit.name">
    <p>Frut: {{ objectFruit.name }}</p>
    <li v-for="(value, key) in objectFruit" :key="key">
      {{ key }} : {{ value }}
    </li>
  </ul>
</template>
