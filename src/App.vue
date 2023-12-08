<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/cube">Cube</RouterLink>
        <RouterLink to="/xr-cube">XR Cube</RouterLink>
        <RouterLink to="/xr-model">XR Model</RouterLink>
        <RouterLink to="/xr-model-overlay">XR Model Overlay</RouterLink>
        <RouterLink to="/xr-gallery">XR Gallery</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>


<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  font-size: 12px;
  text-align: center;
  padding: 16px;
}

nav a.router-link-exact-active {
  color: #FFFFFF;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid rgba(60, 60, 60, 0.66);
  color: rgba(255, 255, 255, 0.29);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    justify-content: center;
    width: 100%;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
  }
}
</style>

