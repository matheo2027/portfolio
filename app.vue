<template>
  <div class="app-container">
    <!-- Barre de navigation -->
    <NavBar />

    <!-- Contenu des pages -->
    <main class="main-content">
      <NuxtPage />
    </main>

    <!-- Pied de page -->
    <Footer />
  </div>
</template>

<script setup>
import NavBar from '~/components/NavBar.vue';
import Footer from '~/components/Footer.vue';
</script>

<style>
/* Styles globaux */
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
  flex: 1; /* Permet au contenu de prendre tout l'espace disponible */
  padding: 2rem;
}
</style>