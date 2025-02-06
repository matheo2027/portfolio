<template>
  <div>
    <h1>Mes projets</h1>
    <ul>
      <li>Projet 1</li>
      <li>Projet 2</li>
      <li>Projet 3</li>
    </ul>
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

  ul {
    list-style: none;
    text-align: center;
    padding: 0;
  }

  li {
    margin: 1rem 0;
  }
</style>