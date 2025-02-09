<template>
    <div class="area-project">
      <header class="area-header">
        <h1 class="area-title">Projet AREA</h1>
      </header>

      <section class="area-description">
        <h2 class="section-title">Qu'est-ce que le projet AREA ?</h2>
        <p class="section-text">
          Le projet AREA est une plateforme innovante conçue pour
          simplifier et automatiser les tâches quotidiennes en connectant différents services et applications. Grâce à
          des workflows personnalisables, AREA permet aux utilisateurs de créer des enchaînements d'actions déclenchées
          par des événements spécifiques.
        </p>
      </section>

      <section class="area-features">
        <h2 class="section-title">Fonctionnalités principales</h2>
        <ul class="features-list">
          <li class="feature-item">
            <strong>Intégration de services multiples :</strong> Connexion à des services populaires comme Google, GitHub, Discord.
          </li>
          <li class="feature-item">
            <strong>Workflows personnalisables :</strong> Créez des enchaînements d'actions en fonction de déclencheurs
            spécifiques.
          </li>
          <li class="feature-item">
            <strong>Automatisation intelligente :</strong> Gagnez du temps en automatisant des tâches répétitives.
          </li>
          <li class="feature-item">
            <strong>Interface intuitive :</strong> Une interface utilisateur simple et conviviale pour configurer et
            gérer vos workflows.
          </li>
        </ul>
      </section>

      <section class="area-use-cases">
        <h2 class="section-title">Cas d'utilisation</h2>
        <div class="use-case">
          <h3 class="use-case-title">Exemple 1 : Notification automatique</h3>
          <p class="use-case-text">
            Recevez une notification par e-mail chaque fois qu'une étoile est mise sur un dépot GitHub.
          </p>
        </div>
        <div class="use-case">
          <h3 class="use-case-title">Exemple 2 : Notifications pour un message reçu</h3>
          <p class="use-case-text">
            Recevez un mail à chaque fois que vous recevez un message dans un serveur Discord.
          </p>
        </div>
      </section>

      <section class="area-technologies">
        <h2 class="section-title">Technologies utilisées</h2>
        <ul class="technologies-list">
          <li class="technology-item">Next.js</li>
          <li class="technology-item">Express.js</li>
          <li class="technology-item">PostgreSQL</li>
          <li class="technology-item">Docker</li>
          <li class="technology-item">API REST</li>
          <li class="technology-item">OAuth 2.0</li>
        </ul>
      </section>

      <footer class="area-footer">
        <p class="footer-text">
          Pour en savoir plus sur le projet AREA, visitez notre
          <a href="https://github.com/matheo2027/AREA" target="_blank" class="footer-link">dépôt GitHub</a>.
        </p>
      </footer>
    </div>
  </template>

  <style scoped>
  .area-project {
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
    font-family: Arial, sans-serif;
    color: #333;
  }

  .area-header {
    text-align: center;
    margin-bottom: 2rem;
  }

  .area-title {
    font-size: 2.5rem;
    color: #00bcd4;
  }

  .area-subtitle {
    font-size: 1.2rem;
    color: #666;
  }

  .section-title {
    font-size: 1.8rem;
    color: #00bcd4;
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

  .use-case {
    margin-bottom: 1.5rem;
  }

  .use-case-title {
    font-size: 1.4rem;
    color: #00bcd4;
    margin-bottom: 0.5rem;
  }

  .use-case-text {
    font-size: 1.1rem;
    line-height: 1.6;
  }

  .area-footer {
    text-align: center;
    margin-top: 3rem;
    padding-top: 1rem;
    border-top: 1px solid #ddd;
  }

  .footer-text {
    font-size: 1rem;
    color: #666;
  }

  .footer-link {
    color: #00bcd4;
    text-decoration: none;
  }

  .footer-link:hover {
    text-decoration: underline;
  }
  </style>