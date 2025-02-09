<template>
  <div class="contact-page">
    <header class="contact-header">
      <h1 class="contact-title">Contact</h1>
      <p class="contact-subtitle">N'hésitez pas à me contacter pour discuter de projets ou de collaborations.</p>
    </header>

    <section class="contact-info">
      <h2 class="section-title">Mes coordonnées</h2>
      <ul class="contact-list">
        <li class="contact-item">
          <span class="contact-icon">📞</span>
          <strong>Téléphone : </strong>
          <a href="tel:+33777083243" class="contact-link">+33 7 77 08 32 43</a>
        </li>
        <li class="contact-item">
          <span class="contact-icon">✉️</span>
          <strong>E-mail : </strong>
          <a href="mailto:matheo.piques@epitech.eu" class="contact-link">matheo.piques@epitech.eu</a>
        </li>
      </ul>
    </section>

    <footer class="contact-footer">
      <p class="footer-text">
        Vous pouvez également me retrouver sur
        <a href="https://github.com/matheo2027" target="_blank" class="footer-link">GitHub</a> et
        <a href="https://www.linkedin.com/in/math%C3%A9o-piques-521805263/" target="_blank" class="footer-link">LinkedIn</a>.
      </p>
    </footer>
  </div>
</template>

<style scoped>
.contact-page {
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

.contact-header {
  text-align: center;
  margin-bottom: 2rem;
}

.contact-title {
  font-size: 2.5rem;
  color: #00bcd4;
  margin-bottom: 0.5rem;
  animation: fadeIn 1s ease-in-out;
}

.contact-subtitle {
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

.contact-list {
  list-style: none;
  padding: 0;
}

.contact-item {
  font-size: 1.1rem;
  margin-bottom: 1.5rem;
  display: flex;
  align-items: center;
  gap: 10px;
  animation: fadeIn 2.5s ease-in-out;
}

.contact-icon {
  font-size: 1.5rem;
  color: #00bcd4;
}

.contact-link {
  color: #00bcd4;
  text-decoration: none;
  transition: color 0.3s ease;
}

.contact-link:hover {
  color: #0097a7;
  text-decoration: underline;
}

.contact-footer {
  text-align: center;
  margin-top: 3rem;
  padding-top: 1rem;
  border-top: 1px solid #ddd;
  animation: fadeIn 3s ease-in-out;
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