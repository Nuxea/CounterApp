<script setup>
  import {ref} from "vue";

  let count = ref(0)
</script>

<template>
  <main>
    <container class="container">
      <h4>The current count is...</h4>
      <h1>{{count}}</h1>
      <div class="buttons">
        <button @click="count--">-</button>
        <button @click="count++">+</button>
      </div>

    </container>
  </main>
</template>

<style scoped>
main {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  text-align: center;
}

.buttons {
  display: flex;
  justify-content: space-evenly;
  gap: 30px;
}

button {
  padding: 10px;
  width: 100px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button:hover {
  background-color: var(--vt-c-text-dark-1);
}
</style>
