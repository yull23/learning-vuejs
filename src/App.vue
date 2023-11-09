<script>
export default {
  methods: {
    handleCLick() {
      console.log("Click");
    },
    handleCLick2(x) {
      console.log(`Click in button ${x}`)
    }
  }
}
</script>

<template>
  <button @click="handleCLick">
    Click me!
  </button>
  <p>According to click</p>
  <button @click.right.prevent="handleCLick2(1)">Button 1</button>
  <button @click="handleCLick2(2)">Button 2</button>
  <button @click.middle="handleCLick2(3)">Button 3</button>
</template>