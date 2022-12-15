<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="primary-header">
    <div class="container">
      <div class="nav-wrapper">
        <img class="logo" src="@/assets/images/Doedactiek-logo.png" alt="Doedactiek logo">
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
    test
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

.nav-wrapper a {
  text-decoration: none;
}

.nav-wrapper {
  display: flex;
  justify-content: space-between;
}

footer {
  background-color: var(--clr-primary-60);
  position: absolute;
  bottom: 0;
  width: 100%;
}
</style>
