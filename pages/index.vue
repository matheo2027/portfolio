<template>
  <div class="home">
    <section class="hero">
      <div class="hero-content">
        <h1 class="hero-title">Bienvenue sur mon portfolio</h1>
        <p class="hero-subtitle">Jeune développeur passionné par la création de solutions web modernes et performantes.</p>
      </div>
    </section>

    <section class="about">
      <div class="about-container">
        <h2 class="about-title">À propos de moi</h2>
        <p class="about-text">
          Je suis un jeune développeur étudiant à l'école Epitech. J'ai une passion pour la création de sites web modernes et performants.
          J'aime travailler sur des projets variés, de la conception à la mise en ligne. Je suis toujours à la recherche de nouveaux défis et de nouvelles technologies à apprendre.
        </p>
        <NuxtLink to="/about" class="about-button">Découvrir qui je suis</NuxtLink>
      </div>
    </section>

    <section class="projects">
      <h2 class="projects-title">Projets récents</h2>
      <div class="projects-grid">
        <div class="project-card">
          <h3 class="project-title">Site web</h3>
          <p class="project-description">
            Un site web complet qui permet de relier des services entre eux, en créant des AREA.
          </p>
          <NuxtLink to="/projets/web" class="project-button">Voir le projet</NuxtLink>
        </div>
        <div class="project-card">
          <h3 class="project-title">Re-création du "ls"</h3>
          <p class="project-description">
            Re-création de la commande "ls" en C.
          </p>
          <NuxtLink to="/projets/ls" class="project-button">Voir le projet</NuxtLink>
        </div>
        <div class="project-card">
          <h3 class="project-title">Projets Graphiques</h3>
          <p class="project-description">
            Création d'un émulateur de borne d'arcade en C++ qui comprends plusieurs jeux.
          </p>
          <NuxtLink to="/projets/graphique" class="project-button">Voir le projet</NuxtLink>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  gap: 4rem;
  padding: 2rem;
}

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