<script setup lang="ts">
import { sum, divide, multiply, subtract, square } from 'procgen'
</script>

<template>
  <div class="about">
    <div>
      <h1>This is a secret page</h1>

      <p>Let's do some <b>more</b> math... with wasm!</p>
      <p>3 + 4 = {{ sum(3, 4) }}</p>
      <p>5 - 4 = {{ subtract(5, 4) }}</p>
      <p>4 * 5 = {{ multiply(4, 5) }}</p>
      <p>9 / 4 = {{ divide(9, 4) }}</p>
      <p>3 ^ 2 = {{ square(3) }}</p>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  secret {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
