<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="wrapper"></div>
  </header>

  <RouterView />
</template>

<style scoped>
nav {
  text-align: center;
}
nav * {
  border: solid 1px black;
  background-color: aquamarine;
}
</style>
