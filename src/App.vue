<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <img class="logo" src="@/assets/images/Doedactiek-logo.png" alt="Doedactiek logo">

    <div class="wrapper">
      <nav class="primary-nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/kerst">Kerst</RouterLink>
        <RouterLink to="/oud-en-nieuw">Oud en nieuw</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />

  <footer>
    <div class="container">
        test
    </div>
  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
  width: 100%;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  width: 160px;
}

.primary-nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

footer {
  background-color: var(--clr-primary-60);
  color: var(--clr-accent-100);
  position: absolute;
  bottom: 0;
  width: 100%;
}
</style>
