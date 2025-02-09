<template>
  <footer class="footer">
    <div class="footer-container">
      <div class="footer-section">
        <h3 class="footer-title">Mon Portfolio</h3>
        <p class="footer-text">Créé par moi, pour moi.</p>
      </div>
      <div class="footer-section">
        <h4 class="footer-subtitle">Liens rapides</h4>
        <ul class="footer-links">
          <li><NuxtLink to="/" class="footer-link">Accueil</NuxtLink></li>
          <li><NuxtLink to="/about" class="footer-link">À propos</NuxtLink></li>
          <li><NuxtLink to="/contact" class="footer-link">Contact</NuxtLink></li>
        </ul>
      </div>
      <div class="footer-section">
        <h4 class="footer-subtitle">Réseaux sociaux</h4>
        <div class="social-links">
          <a href="https://github.com/matheo2027" target="_blank" class="footer-link">GitHub</a>
          <a href="https://www.linkedin.com/in/math%C3%A9o-piques-521805263/" target="_blank" class="footer-link">LinkedIn</a>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2025 Mon Portfolio. Tous droits réservés.</p>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #1a1a1a;
  color: #fff;
  padding: 2rem 0;
  width: 100%;
  margin-top: auto;
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
  color: #00bcd4;
}

.social-links {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.footer-bottom {
  text-align: center;
  margin-top: 2rem;
  padding-top: 1rem;
  border-top: 1px solid #333;
}
</style>