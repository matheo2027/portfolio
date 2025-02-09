<template>
  <div class="about-page">
    <header class="about-header">
      <h1 class="about-title">À propos de moi</h1>
      <p class="about-subtitle">Développeur passionné, étudiant et amateur de défis techniques</p>
    </header>

    <section class="about-description">
      <h2 class="section-title">Qui suis-je ?</h2>
      <p class="section-text">
        Je suis un jeune développeur étudiant à l'école <strong>Epitech Bordeaux</strong>, où j'apprends à maîtriser les
        technologies modernes et à résoudre des problèmes complexes. Ma passion pour le développement web et logiciel
        m'a conduit à travailler sur des projets variés, allant de la conception à la mise en ligne. J'aime créer des
        sites web modernes, performants et accessibles, en utilisant les dernières technologies disponibles.
      </p>
      <p class="section-text">
        Toujours à la recherche de nouveaux défis, je suis constamment en train d'apprendre et d'expérimenter avec de
        nouveaux outils et langages de programmation. Pour moi, chaque projet est une opportunité de progresser et de
        repousser mes limites.
      </p>
    </section>

    <section class="about-passions">
      <h2 class="section-title">Mes passions</h2>
      <ul class="passions-list">
        <li class="passion-item">
          <span class="passion-icon">🚗</span>
          <strong>L'automobile:</strong> Je suis fasciné par l'ingénierie automobile et les innovations dans ce domaine.
          J'aime suivre l'actualité des voitures de sport et des technologies de pointe.
        </li>
        <li class="passion-item">
          <span class="passion-icon">⚽</span>
          <strong>Le sport:</strong> Que ce soit en pratiquant ou en regardant, le sport fait partie de ma vie. Le
          football et le rugby sont mes préférés.
        </li>
        <li class="passion-item">
          <span class="passion-icon">🍲</span>
          <strong>La nourriture:</strong> Gourmand dans l'âme, j'adore découvrir de nouvelles cuisines et expérimenter
          des recettes en cuisine.
        </li>
        <li class="passion-item">
          <span class="passion-icon">💻</span>
          <strong>Le code:</strong> Le développement est bien plus qu'un métier pour moi, c'est une passion. J'aime
          créer des solutions innovantes et résoudre des problèmes complexes.
        </li>
        <li class="passion-item">
          <span class="passion-icon">🎮</span>
          <strong>Les jeux vidéo:</strong> Fan de jeux rétro et modernes, j'apprécie autant y jouer qu'analyser leur
          conception et leur gameplay.
        </li>
      </ul>
    </section>

    <section class="about-skills">
      <h2 class="section-title">Mes compétences</h2>
      <ul class="skills-list">
        <li class="skill-item">
          <span class="skill-icon">🌐</span>
          Développement web (HTML, CSS, JavaScript, Typescript, Nuxt.js, Next.js, Express.js, Angular)
        </li>
        <li class="skill-item">
          <span class="skill-icon">🖥️</span>
          Développement logiciel (C, C++)
        </li>
        <li class="skill-item">
          <span class="skill-icon">🗄️</span>
          Gestion de bases de données (SQL)
        </li>
        <li class="skill-item">
          <span class="skill-icon">🔧</span>
          Outils de versioning (Git, GitHub)
        </li>
      </ul>
    </section>

    <section class="about-goals">
      <h2 class="section-title">Mes objectifs</h2>
      <p class="section-text">
        Mon objectif est de devenir un développeur full-stack polyvalent, capable de travailler sur tous les aspects
        d'un projet, du front-end au back-end. Je souhaite également contribuer à des projets open-source et continuer
        à apprendre des nouvelles technologies comme l'intelligence artificielle et le développement de jeux vidéo.
      </p>
    </section>

    <section class="about-cv">
      <h2 class="section-title">Mon CV</h2>
      <p class="section-text">
        Vous pouvez consulter et télécharger mon CV pour en savoir plus sur mon parcours et mes compétences.
      </p>

      <div class="cv-preview">
        <img src="/CV-preview.png" alt="Aperçu du CV" class="cv-image" />
      </div>

      <a href="/CV.pdf" download class="cv-link">Télécharger mon CV</a>
    </section>

    <footer class="about-footer">
      <p class="footer-text">
        Vous voulez en savoir plus ? N'hésitez pas à me contacter via
        <a href="/contact" class="footer-link">la page de contact</a>.
      </p>
    </footer>
  </div>
</template>

<style scoped>
.about-page {
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

.about-header {
  text-align: center;
  margin-bottom: 2rem;
}

.about-title {
  font-size: 2.5rem;
  color: #00bcd4;
  margin-bottom: 0.5rem;
  animation: fadeIn 1s ease-in-out;
}

.about-subtitle {
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

.passions-list,
.skills-list {
  list-style: none;
  padding: 0;
}

.passion-item,
.skill-item {
  font-size: 1.1rem;
  margin-bottom: 1.5rem;
  display: flex;
  align-items: center;
  gap: 10px;
  animation: fadeIn 3s ease-in-out;
}

.passion-icon,
.skill-icon {
  font-size: 1.5rem;
  color: #00bcd4;
}

.about-cv {
  text-align: center;
  margin-top: 3rem;
  padding-top: 1rem;
  border-top: 1px solid #ddd;
  animation: fadeIn 4s ease-in-out;
}

.cv-preview {
  margin: 2rem 0;
  text-align: center;
}

.cv-image {
  max-width: 100%;
  height: auto;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.cv-image:hover {
  transform: scale(1.02);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

.cv-link {
  display: inline-block;
  background-color: #00bcd4;
  color: #fff;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  text-decoration: none;
  font-size: 1.1rem;
  transition: background-color 0.3s ease;
  margin-top: 1rem;
}

.cv-link:hover {
  background-color: #0097a7;
}

.about-footer {
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

.footer-link {
  color: #00bcd4;
  text-decoration: none;
  transition: color 0.3s ease;
}

.footer-link:hover {
  color: #0097a7;
  text-decoration: underline;
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