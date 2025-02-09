<template>
  <div class="ls-project">
    <header class="ls-header">
      <h1 class="ls-title">Projet my_ls</h1>
    </header>

    <section class="ls-description">
      <h2 class="section-title">Qu'est-ce que my_ls ?</h2>
      <p class="section-text">
        Le projet <strong>my_ls</strong> est une réimplémentation en langage C de la commande Unix <code>ls</code>,
        utilisée pour lister les fichiers et répertoires dans un dossier. Ce projet a été développé dans le but de
        comprendre en profondeur le fonctionnement des appels système et de manipuler les structures de données en C.
      </p>
    </section>

    <section class="ls-features">
      <h2 class="section-title">Fonctionnalités implémentées</h2>
      <ul class="features-list">
        <li class="feature-item">
          <span class="feature-icon">📄</span>
          <strong>Liste simple :</strong> Affiche les fichiers et répertoires dans le dossier courant.
        </li>
        <li class="feature-item">
          <span class="feature-icon">🔍</span>
          <strong>Options de tri :</strong> Tri des fichiers par nom, date de modification, taille, etc.
        </li>
        <li class="feature-item">
          <span class="feature-icon">📊</span>
          <strong>Affichage détaillé :</strong> Affiche les permissions, propriétaire, groupe, taille et date de
          modification des fichiers.
        </li>
        <li class="feature-item">
          <span class="feature-icon">⚙️</span>
          <strong>Gestion des options :</strong> Support des options courantes comme <code>-l</code>, <code>-a</code>,
          <code>-R</code>, etc.
        </li>
      </ul>
    </section>

    <section class="ls-technologies">
      <h2 class="section-title">Technologies utilisées</h2>
      <ul class="technologies-list">
        <li class="technology-item">
          <span class="technology-icon">💻</span>
          Langage C
        </li>
        <li class="technology-item">
          <span class="technology-icon">📂</span>
          Appels système Unix (stat, opendir, readdir, etc.)
        </li>
        <li class="technology-item">
          <span class="technology-icon">🔧</span>
          Makefile pour la compilation
        </li>
      </ul>
    </section>

    <section class="ls-examples">
      <h2 class="section-title">Exemples d'utilisation</h2>
      <div class="example">
        <h3 class="example-title">Liste simple</h3>
        <pre class="example-code"><code>$ ./my_ls
file1.txt  file2.txt  directory1  directory2</code></pre>
      </div>
      <div class="example">
        <h3 class="example-title">Affichage détaillé</h3>
        <pre class="example-code"><code>$ ./my_ls -l
-rw-r--r-- 1 user group  4096 Oct  1 12:34 file1.txt
drwxr-xr-x 2 user group  4096 Oct  1 12:34 directory1</code></pre>
      </div>
    </section>

    <footer class="ls-footer">
      <p class="footer-text">
        Pour en savoir plus sur le projet my_ls, visitez notre
        <a href="https://github.com/matheo2027/my_ls" target="_blank" class="footer-link">dépôt GitHub</a>.
      </p>
    </footer>
  </div>
</template>

<style scoped>
.ls-project {
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

.ls-header {
  text-align: center;
  margin-bottom: 2rem;
}

.ls-title {
  font-size: 2.5rem;
  color: #00bcd4;
  margin-bottom: 0.5rem;
  animation: fadeIn 1s ease-in-out;
}

.ls-subtitle {
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

.example-code {
  background-color: #f5f5f5;
  padding: 1rem;
  border-radius: 4px;
  font-family: "Courier New", monospace;
  font-size: 1rem;
  overflow-x: auto;
}

.ls-footer {
  text-align: center;
  margin-top: 3rem;
  padding-top: 1rem;
  border-top: 1px solid #ddd;
  animation: fadeIn 4s ease-in-out;
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