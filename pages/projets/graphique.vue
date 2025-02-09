<template>
  <div class="arcade-project">
    <header class="arcade-header">
      <h1 class="arcade-title">Projet Arcade</h1>
    </header>

    <section class="arcade-description">
      <h2 class="section-title">Qu'est-ce que le projet Arcade ?</h2>
      <p class="section-text">
        Le projet <strong>Arcade</strong> est un moteur graphique conçu pour développer des jeux vidéo rétro inspirés
        des années 80 et 90. Ce projet permet de créer des jeux en 2D avec des graphismes pixelisés, des animations
        fluides et une gestion des entrées utilisateur. Il est idéal pour les passionnés de développement de jeux et
        les amateurs de nostalgie.
      </p>
    </section>

    <section class="arcade-features">
      <h2 class="section-title">Fonctionnalités principales</h2>
      <ul class="features-list">
        <li class="feature-item">
          <span class="feature-icon">🎮</span>
          <strong>Rendu graphique 2D :</strong> Affichage de sprites, tilesets et animations.
        </li>
        <li class="feature-item">
          <span class="feature-icon">⌨️</span>
          <strong>Gestion des entrées :</strong> Prise en charge du clavier.
        </li>
        <li class="feature-item">
          <span class="feature-icon">🎵</span>
          <strong>Gestion du son :</strong> Lecture de musiques et effets sonores en format chiptune.
        </li>
        <li class="feature-item">
          <span class="feature-icon">🧩</span>
          <strong>Modularité :</strong> Architecture modulaire pour ajouter facilement de nouvelles fonctionnalités.
        </li>
      </ul>
    </section>

    <section class="arcade-technologies">
      <h2 class="section-title">Technologies utilisées</h2>
      <ul class="technologies-list">
        <li class="technology-item">
          <span class="technology-icon">💻</span>
          C++ (langage principal)
        </li>
        <li class="technology-item">
          <span class="technology-icon">🛠️</span>
          SFML (Simple and Fast Multimedia Library)
        </li>
        <li class="technology-item">
          <span class="technology-icon">🖥️</span>
          OpenGL (pour le rendu avancé)
        </li>
        <li class="technology-item">
          <span class="technology-icon">🔧</span>
          CMake (pour la gestion de la compilation)
        </li>
      </ul>
    </section>

    <section class="arcade-examples">
      <h2 class="section-title">Exemples de jeux créés avec Arcade</h2>
      <div class="example">
        <h3 class="example-title">Snake</h3>
        <p class="example-text">
          Un classique indémodable où vous contrôlez un serpent qui grandit en mangeant des fruits. Attention à ne pas
          heurter les murs ou votre propre queue !
        </p>
      </div>
      <div class="example">
        <h3 class="example-title">Pacman</h3>
        <p class="example-text">
          Incarnez Pacman et parcourez le labyrinthe pour manger toutes les pac-gommes tout en évitant les fantômes.
          Utilisez les super pac-gommes pour les rendre vulnérables !
        </p>
      </div>
      <div class="example">
        <h3 class="example-title">Nibbler</h3>
        <p class="example-text">
          Un jeu de serpent amélioré où vous devez manger des fruits pour grandir tout en évitant les obstacles et en
          planifiant vos mouvements dans un espace limité.
        </p>
      </div>
    </section>

    <section class="arcade-get-started">
      <h2 class="section-title">Comment commencer ?</h2>
      <p class="section-text">
        Pour utiliser le moteur Arcade, clonez le dépôt GitHub et suivez les instructions du README pour configurer
        votre environnement de développement. Des exemples de jeux sont fournis pour vous aider à démarrer.
      </p>
    </section>

    <footer class="arcade-footer">
        <p class="footer-text">
          Pour en savoir plus sur le projet Arcade, visitez notre
          <a href="https://github.com/matheo2027/Arcade" target="_blank" class="footer-link">dépôt GitHub</a>.
        </p>
      </footer>
  </div>
</template>

<style scoped>
.arcade-project {
  max-width: 800px;
  margin: 0 auto;
  margin-top: 3%;
  padding: 2rem;
  font-family: Arial, sans-serif;
  color: #333;
  background-color: #f9f9f9;
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.arcade-header {
  text-align: center;
  margin-bottom: 2rem;
}

.arcade-title {
  font-size: 2.5rem;
  color: #00bcd4;
  margin-bottom: 0.5rem;
  animation: fadeIn 1s ease-in-out;
}

.arcade-subtitle {
  font-size: 1.2rem;
  color: #666;
  animation: fadeIn 1.5s ease-in-out;
}

.section-title {
  font-size: 1.8rem;
  color: #00bcd4;
  margin-bottom: 1.5rem;
  animation: fadeIn 2s ease-in-out;
}

.section-text {
  font-size: 1.1rem;
  line-height: 1.6;
  margin-bottom: 2rem;
  animation: fadeIn 2.5s ease-in-out;
}

.features-list,
.technologies-list {
  list-style: none;
  padding: 0;
}

.feature-item,
.technology-item {
  font-size: 1.1rem;
  margin-bottom: 1.5rem;
  display: flex;
  align-items: center;
  gap: 10px;
  animation: fadeIn 3s ease-in-out;
}

.feature-icon,
.technology-icon {
  font-size: 1.5rem;
  color: #00bcd4;
}

.example {
  margin-bottom: 1.5rem;
  animation: fadeIn 3.5s ease-in-out;
}

.example-title {
  font-size: 1.4rem;
  color: #00bcd4;
  margin-bottom: 0.5rem;
}

.example-text {
  font-size: 1.1rem;
  line-height: 1.6;
}

.get-started-link {
  display: inline-block;
  background-color: #00bcd4;
  color: #fff;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  text-decoration: none;
  font-size: 1.1rem;
  transition: background-color 0.3s ease;
  animation: fadeIn 4s ease-in-out;
}

.get-started-link:hover {
  background-color: #0097a7;
}

.footer-link {
    color: #00bcd4;
    text-decoration: none;
  }

  .footer-link:hover {
    text-decoration: underline;
  }

.arcade-footer {
  text-align: center;
  margin-top: 3rem;
  padding-top: 1rem;
  border-top: 1px solid #ddd;
  animation: fadeIn 4.5s ease-in-out;
}

.footer-text {
  font-size: 1rem;
  color: #666;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>