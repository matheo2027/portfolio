<template>
  <footer class="footer">
    <div class="footer-container">
      <div class="footer-section">
        <h3 class="footer-title">Mon Portfolio</h3>
        <p class="footer-text">Créé avec passion et dévouement.</p>
      </div>
      <div class="footer-section">
        <h4 class="footer-subtitle">Liens rapides</h4>
        <ul class="footer-links">
          <li><NuxtLink to="/" class="footer-link">Accueil</NuxtLink></li>
          <li><NuxtLink to="/about" class="footer-link">À propos</NuxtLink></li>
          <li><NuxtLink to="/projects" class="footer-link">Projets</NuxtLink></li>
          <li><NuxtLink to="/contact" class="footer-link">Contact</NuxtLink></li>
        </ul>
      </div>
      <div class="footer-section">
        <h4 class="footer-subtitle">Réseaux sociaux</h4>
        <div class="social-icons">
          <a href="https://twitter.com" target="_blank" class="social-icon">
            <i class="fab fa-twitter"></i>
          </a>
          <a href="https://github.com" target="_blank" class="social-icon">
            <i class="fab fa-github"></i>
          </a>
          <a href="https://linkedin.com" target="_blank" class="social-icon">
            <i class="fab fa-linkedin"></i>
          </a>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2023 Mon Portfolio. Tous droits réservés.</p>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #1a1a1a;
  color: #fff;
  padding: 2rem 0;
  width: 100%; /* Occuper toute la largeur */
  margin-top: auto; /* Pousser le footer en bas */
}

.footer-container {
  display: flex;
  justify-content: space-around;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

.footer-section {
  flex: 1;
  margin: 0 1rem;
}

.footer-title {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

.footer-subtitle {
  font-size: 1.2rem;
  margin-bottom: 1rem;
}

.footer-links {
  list-style: none;
  padding: 0;
}

.footer-link {
  color: #fff;
  text-decoration: none;
  display: block;
  margin-bottom: 0.5rem;
  transition: color 0.3s ease;
}

.footer-link:hover {
  color: #00bcd4; /* Couleur au survol */
}

.social-icons {
  display: flex;
  gap: 1rem;
}

.social-icon {
  color: #fff;
  font-size: 1.5rem;
  transition: color 0.3s ease;
}

.social-icon:hover {
  color: #00bcd4; /* Couleur au survol */
}

.footer-bottom {
  text-align: center;
  margin-top: 2rem;
  padding-top: 1rem;
  border-top: 1px solid #333;
}
</style>