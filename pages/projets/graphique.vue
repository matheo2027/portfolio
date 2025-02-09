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
            <strong>Rendu graphique 2D :</strong> Affichage de sprites, tilesets et animations.
          </li>
          <li class="feature-item">
            <strong>Gestion des entrées :</strong> Prise en charge du clavier.
          </li>
          <li class="feature-item">
            <strong>Gestion du son :</strong> Lecture de musiques et effets sonores en format chiptune.
          </li>
          <li class="feature-item">
            <strong>Modularité :</strong> Architecture modulaire pour ajouter facilement de nouvelles fonctionnalités.
          </li>
        </ul>
      </section>

      <section class="arcade-technologies">
        <h2 class="section-title">Technologies utilisées</h2>
        <ul class="technologies-list">
          <li class="technology-item">C++ (langage principal)</li>
          <li class="technology-item">SFML (Simple and Fast Multimedia Library)</li>
          <li class="technology-item">OpenGL (pour le rendu avancé)</li>
          <li class="technology-item">CMake (pour la gestion de la compilation)</li>
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
    padding: 2rem;
    font-family: Arial, sans-serif;
    color: #333;
  }

  .arcade-header {
    text-align: center;
    margin-bottom: 2rem;
  }

  .arcade-title {
    font-size: 2.5rem;
    color: #00bcd4; /* Couleur turquoise pour correspondre au style des autres pages */
  }

  .arcade-subtitle {
    font-size: 1.2rem;
    color: #666;
  }

  .section-title {
    font-size: 1.8rem;
    color: #00bcd4; /* Couleur turquoise pour les titres */
    margin-bottom: 1rem;
  }

  .section-text {
    font-size: 1.1rem;
    line-height: 1.6;
    margin-bottom: 2rem;
  }

  .features-list,
  .technologies-list {
    list-style: none;
    padding: 0;
  }

  .feature-item,
  .technology-item {
    font-size: 1.1rem;
    margin-bottom: 0.8rem;
  }

  .example {
    margin-bottom: 1.5rem;
  }

  .example-title {
    font-size: 1.4rem;
    color: #00bcd4; /* Couleur turquoise pour les sous-titres */
    margin-bottom: 0.5rem;
  }

  .example-text {
    font-size: 1.1rem;
    line-height: 1.6;
  }

  .footer-link {
    color: #00bcd4; /* Couleur turquoise pour les liens */
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
  }

  .footer-text {
    font-size: 1rem;
    color: #666;
  }
  </style>