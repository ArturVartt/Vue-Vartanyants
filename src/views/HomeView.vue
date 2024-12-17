<script></script>

<template>
  <div class="home-page">
    <header class="header">
      <h1>Добро пожаловать в наш магазин картин!</h1>
      <nav class="navbar">
        <ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
          <li><RouterLink to="/gallery">Gallery</RouterLink></li>
        </ul>
      </nav>
    </header>

    <main class="main-content">
      <section class="intro">
        <h2>Откройте мир искусства</h2>
        <p>
          Мы предлагаем вам уникальные картины для любого интерьера. Найдите
          произведения искусства, которые вдохновляют и подчеркивают вашу
          индивидуальность.
        </p>
      </section>

      <section class="featured">
        <h2>Популярные картины</h2>
        <div class="product-list">
          <div
            class="product-card"
            v-for="(product, index) in products"
            :key="index"
          >
            <h3>{{ product.name }}</h3>
            <p>{{ product.description }}</p>
            <p>
              <strong>{{ product.price }} ₽</strong>
            </p>
            <button @click="addToCart(product)">Добавить в корзину</button>
          </div>
        </div>
      </section>
    </main>

    <footer class="footer">
      <p>&copy; 2024 Магазин картин. Все права защищены.</p>
    </footer>
  </div>
</template>
<style scoped>
.home-page {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

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

.main-content {
  padding: 20px;
}

.intro {
  text-align: center;
  margin-bottom: 40px;
}

.featured h2 {
  text-align: center;
}

.product-list {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.product-card {
  background-color: white;
  padding: 15px;
  margin: 10px;
  width: 250px;
  border: 1px solid #ddd;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.product-card h3 {
  font-size: 18px;
  margin-bottom: 10px;
}

.product-card p {
  font-size: 14px;
  margin-bottom: 10px;
}

.product-card button {
  background-color: #28a745;
  color: white;
  border: none;
  padding: 10px 15px;
  cursor: pointer;
  font-size: 14px;
}

.product-card button:hover {
  background-color: #218838;
}

.footer {
  text-align: center;
  padding: 20px;
  background-color: #333;
  color: white;
}

footer p {
  margin: 0;
}
</style>
