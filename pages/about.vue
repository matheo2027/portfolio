<template>
  <div>
    <h1>À propos de moi</h1>
    <p>Je suis un développeur passionné par la création de sites web modernes.</p>
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