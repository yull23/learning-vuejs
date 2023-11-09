<script setup>
const name = "Vue 3";
const arrayFruts = [
  {
    name: "Manzana",
    price: "$1.00",
    description: "Una manzana",
  },
  {
    name: "Pera",
    price: "$2.00",
    description: "Una pera",
  },
  {
    name: "Naranja",
    price: "$3.00",
    description: "Una naranja",
  },
];
</script>
<template>
  <h1>Hola</h1>
  <p>{{ name }}</p>

  <div>
    <ul>
      <li v-for="element in arrayFruts">
        <p>{{ element.name }}</p>
        <p>{{ element.price }}</p>
        <p>{{ element.description }}</p>
      </li>
    </ul>
  </div>
</template>
<style></style>

