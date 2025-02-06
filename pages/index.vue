<template>
  <div>
    <h1>Bienvenue sur mon portfolio</h1>
    <p>Ceci est la page d'accueil de mon portfolio.</p>
  </div>
 </template>

<script>
  import NavBar from '~/components/NavBar.vue';
  import Footer from '~/components/Footer.vue'

  export default {
    components: {
      NavBar,
      Footer
    }
  }
</script>

<style scoped>
  h1 {
    text-align: center;
    margin-top: 2rem;
  }

  p {
    text-align: center;
  }
</style>