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
  <main class="main-content">
    <section class="intro">
      <h2>Наша миссия</h2>
      <p>
        Мы стремимся сделать искусство доступным каждому. В нашем магазине
        представлены картины, которые добавляют теплоту и индивидуальность в
        любой интерьер.
      </p>
    </section>

    <section class="values">
      <h2>Наши ценности</h2>
      <ul>
        <li>
          <strong>Качество:</strong> Каждая картина тщательно отбирается, чтобы
          гарантировать высочайшее качество.
        </li>
        <li>
          <strong>Индивидуальность:</strong> Мы верим в силу уникальных
          произведений искусства, которые подчеркивают характер их владельцев.
        </li>
        <li>
          <strong>Доступность:</strong> Мы делаем искусство доступным для
          широкой аудитории, чтобы каждый мог найти что-то для себя.
        </li>
      </ul>
    </section>

    <section class="team">
      <h2>Наша команда</h2>
      <p>'Иван Иванов'</p>
      <p>'Мария Петрова'</p>
    </section>
  </main>
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
main-content {
  padding: 20px;
}

.intro,
.values,
.team {
  margin-bottom: 40px;
}

h2 {
  text-align: center;
  font-size: 24px;
  color: #333;
}

p {
  font-size: 16px;
  line-height: 1.6;
  text-align: center;
}

.values ul {
  list-style-type: none;
  padding: 0;
  font-size: 16px;
  text-align: left;
  margin-top: 20px;
}

.values li {
  margin-bottom: 10px;
}

.team-members {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.team-member {
  background-color: white;
  padding: 20px;
  margin: 10px;
  width: 250px;
  border: 1px solid #ddd;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.team-member h3 {
  font-size: 18px;
  margin-bottom: 10px;
}

.team-member p {
  font-size: 14px;
  color: #555;
}
</style>
