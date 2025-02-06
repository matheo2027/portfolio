<template>
  <div class="home">
    <!-- Section Hero (Introduction) -->
    <section class="hero">
      <div class="hero-content">
        <h1 class="hero-title">Bienvenue sur mon portfolio</h1>
        <p class="hero-subtitle">Développeur passionné par la création de solutions web modernes et performantes.</p>
        <NuxtLink to="/about" class="hero-button">En savoir plus</NuxtLink>
      </div>
    </section>

    <!-- Section À propos (Présentation) -->
    <section class="about">
      <div class="about-container">
        <h2 class="about-title">À propos de moi</h2>
        <p class="about-text">
          Je suis un développeur full-stack avec une passion pour les technologies web. J'aime créer des applications
          intuitives, performantes et esthétiques. Mon expertise couvre le développement front-end, back-end, et la
          gestion de bases de données.
        </p>
        <NuxtLink to="/about" class="about-button">Découvrir mon parcours</NuxtLink>
      </div>
    </section>

    <!-- Section Projets récents -->
    <section class="projects">
      <h2 class="projects-title">Projets récents</h2>
      <div class="projects-grid">
        <div class="project-card">
          <!-- <img src="/images/project1.jpg" alt="Projet 1" class="project-image" /> -->
          <h3 class="project-title">Site web e-commerce</h3>
          <p class="project-description">
            Un site web e-commerce complet avec gestion de panier, paiement en ligne et tableau de bord administrateur.
          </p>
          <NuxtLink to="/projects/web" class="project-button">Voir le projet</NuxtLink>
        </div>
        <div class="project-card">
          <!-- <img src="/images/project2.jpg" alt="Projet 2" class="project-image" /> -->
          <h3 class="project-title">Application mobile</h3>
          <p class="project-description">
            Une application mobile cross-platform pour la gestion de tâches avec synchronisation en temps réel.
          </p>
          <NuxtLink to="/projects/mobile" class="project-button">Voir le projet</NuxtLink>
        </div>
        <div class="project-card">
          <!-- <img src="/images/project3.jpg" alt="Projet 3" class="project-image" /> -->
          <h3 class="project-title">Design graphique</h3>
          <p class="project-description">
            Conception d'une identité visuelle pour une startup, incluant logo, palette de couleurs et supports de communication.
          </p>
          <NuxtLink to="/projects/design" class="project-button">Voir le projet</NuxtLink>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
// Pas besoin de logique complexe ici
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  gap: 4rem;
  padding: 2rem;
}

/* Section Hero */
.hero {
  background: linear-gradient(135deg, #1a1a1a, #333);
  color: #fff;
  padding: 6rem 2rem;
  text-align: center;
  border-radius: 10px;
}

.hero-content {
  max-width: 800px;
  margin: 0 auto;
}

.hero-title {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.hero-subtitle {
  font-size: 1.25rem;
  margin-bottom: 2rem;
}

.hero-button {
  background: linear-gradient(45deg, #00bcd4, #0097a7);
  color: #fff;
  padding: 0.75rem 1.5rem;
  border-radius: 5px;
  text-decoration: none;
  font-size: 1rem;
  transition: transform 0.3s ease;
}

.hero-button:hover {
  transform: scale(1.05);
}

/* Section À propos */
.about {
  background: #f4f4f4;
  padding: 4rem 2rem;
  text-align: center;
  border-radius: 10px;
}

.about-container {
  max-width: 800px;
  margin: 0 auto;
}

.about-title {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.about-text {
  font-size: 1.1rem;
  margin-bottom: 2rem;
  line-height: 1.6;
}

.about-button {
  background: linear-gradient(45deg, #00bcd4, #0097a7);
  color: #fff;
  padding: 0.75rem 1.5rem;
  border-radius: 5px;
  text-decoration: none;
  font-size: 1rem;
  transition: transform 0.3s ease;
}

.about-button:hover {
  transform: scale(1.05);
}

/* Section Projets */
.projects {
  padding: 4rem 2rem;
  text-align: center;
}

.projects-title {
  font-size: 2.5rem;
  margin-bottom: 2rem;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.project-card {
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease;
}

.project-card:hover {
  transform: translateY(-10px);
}

.project-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.project-title {
  font-size: 1.5rem;
  margin: 1rem 0;
}

.project-description {
  font-size: 1rem;
  padding: 0 1rem;
  margin-bottom: 1rem;
}

.project-button {
  display: inline-block;
  background: linear-gradient(45deg, #00bcd4, #0097a7);
  color: #fff;
  padding: 0.75rem 1.5rem;
  border-radius: 5px;
  text-decoration: none;
  font-size: 1rem;
  margin-bottom: 1rem;
  transition: transform 0.3s ease;
}

.project-button:hover {
  transform: scale(1.05);
}
</style>