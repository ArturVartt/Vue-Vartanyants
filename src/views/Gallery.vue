<script setup>
import { ref } from "vue";

const likes = ref(1);
console.log(likes.value);
function onclick() {
  likes.value++;
}
</script>

<template>
  <header class="header">
    <nav class="navbar">
      <ul>
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/about">About</RouterLink></li>
        <li><RouterLink to="/gallery">Gallery</RouterLink></li>
      </ul>
    </nav>
  </header>
  <h1>Gallery</h1>
  <img
    src="https://i.pinimg.com/736x/fa/7d/7d/fa7d7d0dd96896a6d47f06fd2817ffa7.jpg"
  />
  <div>
    Кол-во лайков:
    <h2>{{ likes }}</h2>
  </div>

  <button v-on:click="onclick">Лайк</button>
</template>

<style scoped>
.header {
  background-color: #333;
  color: white;
  padding: 20px;
  text-align: center;
}

.navbar ul {
  list-style-type: none;
  padding: 0;
}

.navbar li {
  display: inline;
  margin: 0 15px;
}

.navbar a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}
</style>
