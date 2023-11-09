<script setup>
const name = "Vue 3";
const active = true;
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
const number = 2

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
  <div>
    <p v-if="number > 5">Number is greater than 5</p>
    <p v-else-if="number == 5">Number is equal to 5</p>
    <p v-else>Number is less than 5</p>
  </div>
  <div>
    <h2 v-if="active">v-if en acción</h2>
    <h2 v-else>v-else en acción</h2>
  </div>
</template>
<style></style>

