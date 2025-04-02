<script setup lang="ts">
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <header class="header">
    <NavBar></NavBar>
  </header>

  <main>
    <section></section>
    <section></section>
    <section></section>
    <section></section>
  </main>

  <footer>
    <Footer></Footer>
  </footer>
</template>

<style scoped>
  .header {
    height: 8vh;
    background-color: var(--light-rose);
  }

  .footer {
    height: 8vh;    
  }
</style>
