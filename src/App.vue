<script setup lang="ts">
import { RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
import TheNavBar from './components/TheNavBar.vue'
import TheFootBar from './components/TheFootBar.vue'
</script>

<template>
  <header>
    <TheNavBar />
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div> -->
  </header>
  <main>
    <RouterView />
  </main>
  <footer>
    <TheFootBar />
        <!-- <RouterLink to="/about">About</RouterLink> -->
  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
  height: 5.5vh;
}
main {
  flex-grow: 1;
  height: 100%;
}
footer {
  height: 10vh;
}

/* nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
} */

@media (min-width: 1024px) {
  header {
    display: flex;
    justify-content: space-between;
  }
}
</style>
