<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="primary-header">
    <div class="container">
      <div class="nav-wrapper">
        <img class="logo" src="@/assets/images/logo.png" alt="Doedactiek logo">
        <nav class="primary-nav">
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
          <RouterLink to="/kerst">Kerst</RouterLink>
          <RouterLink to="/oud-en-nieuw">Oud en nieuw</RouterLink>
        </nav>
        <RouterLink to="/kerst">Kerst</RouterLink>
      </div>
    </div>
  </header>

  <RouterView />

  <footer>
    <div class="container">
        <div class="footer-wrapper">
          <!-- Col 1 -->
          <div class="footer-logo">
            <img src="@/assets/images/logo-white.png" alt="Doedactiek logo wit">
          </div>
          <!-- Col 2 -->
          <div class="footer-tools">
            <h3>Tools</h3>
            <ul>
              <li><a href="#">Beroepsgericht</a></li>
              <li><a href="#">Creatief</a></li>
              <li><a href="#">Exacte vakken</a></li>
              <li><a href="#">Mentoraat</a></li>
              <li><a href="#">Sportief</a></li>
              <li><a href="#">Talen</a></li>
              <li><a href="#">Zaalvakken</a></li>
            </ul>
          </div>
          <!-- Col 3 -->
          <div>
            <h3>Publicaties</h3>
            <ul>
              <li><a href="#">Onderzoek</a></li>
              <li><a href="#">Dagboek</a></li>
            </ul>
          </div>
          <!-- Col 4 -->
          <div>
            <h3>Ontdek</h3>
            <ul>
              <li><a href="#">Over ons</a></li>
              <li><a href="#">Contact</a></li>
              <li><a href="#">FAQ</a></li>
            </ul>
          </div>
          <!-- Col 5 -->
          <div class="socials">
            <ul>
              <li><a href="#"><i class="fab fa-linkedin-in"></i></a></li>
              <li><a href="#"><i class="fas fa-envelope"></i></a></li>
            </ul>
          </div>
        </div>
    </div>
  </footer>
</template>

<style scoped>

.logo {
  display: block;
  width: 160px;
}

.primary-nav {
  display: flex;
  gap: 1.5em;
}

.nav-wrapper a,
.footer-wrapper a {
  text-decoration: none;
}

.nav-wrapper {
  display: flex;
  justify-content: space-between;
}

footer {
  background-color: var(--clr-primary-60);
  color: var(--clr-accent-100);
  position: relative;
  width: 100%;
}

footer h3 {
  margin-bottom: 20px;
}

footer li {
  list-style: none;
}

footer li a {
  color: var(--clr-accent-100);
}

footer li a:hover {
  color: var(--clr-accent-90);
}

.footer-wrapper {
  padding-top: 50px;
  padding-bottom: 50px;
  display: grid;
  grid-template-columns: 2fr 2fr 1fr 1fr 2fr;
}

.footer-logo {
  display: flex;
  align-items: center;
}

.footer-logo img {
  display: block;
  width: 160px;
}

.footer-tools ul {
  columns: 2;
}

footer .socials {
  display: flex;
  align-items: center;
  justify-content: end;
}

footer .socials ul li {
  display: inline-block;
  font-size: 30px;
}

footer .socials ul li:first-child {
  margin-right: 15px;
}
</style>
