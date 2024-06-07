<script setup lang="ts">
import sayHello from "@shayan/package-a"
const props = defineProps(['text'])
const name = sayHello("shayan")
</script>

<template>
  <button class="btn">click here</button>
</template>

<style scoped>
/* Base button style */
.btn {
  display: inline-block;
  padding: 12px 24px;
  font-size: 16px;
  font-weight: bold;
  text-align: center;
  text-decoration: none;
  color: #fff;
  background-color: #007bff;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.3s, transform 0.3s;
}

/* Button hover effect */
.btn:hover {
  background-color: #0056b3;
}

/* Button active effect */
.btn:active {
  background-color: #004085;
  transform: scale(0.98);
}

/* Button focus effect */
.btn:focus {
  outline: none;
  box-shadow: 0 0 0 3px rgba(38, 143, 255, 0.5);
}

</style>