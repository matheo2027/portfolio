<template>
  <div class="app-container">
    <NavBar />

    <main class="main-content">
      <NuxtPage />
    </main>

    <Footer />
  </div>
</template>

<script setup>
import NavBar from '~/components/NavBar.vue';
import Footer from '~/components/Footer.vue';
</script>

<style>
html, body {
  height: 100%;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  color: #333;
}

.app-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main-content {
  flex: 1;
  padding: 2rem;
  margin-top: 2%;
}
</style>