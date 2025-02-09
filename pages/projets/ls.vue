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
            <strong>Liste simple :</strong> Affiche les fichiers et répertoires dans le dossier courant.
          </li>
          <li class="feature-item">
            <strong>Options de tri :</strong> Tri des fichiers par nom, date de modification, taille, etc.
          </li>
          <li class="feature-item">
            <strong>Affichage détaillé :</strong> Affiche les permissions, propriétaire, groupe, taille et date de
            modification des fichiers.
          </li>
          <li class="feature-item">
            <strong>Gestion des options :</strong> Support des options courantes comme <code>-l</code>, <code>-a</code>,
            <code>-R</code>, etc.
          </li>
        </ul>
      </section>

      <section class="ls-technologies">
        <h2 class="section-title">Technologies utilisées</h2>
        <ul class="technologies-list">
          <li class="technology-item">Langage C</li>
          <li class="technology-item">Appels système Unix (stat, opendir, readdir, etc.)</li>
          <li class="technology-item">Makefile pour la compilation</li>
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
    padding: 2rem;
    font-family: Arial, sans-serif;
    color: #333;
  }

  .ls-header {
    text-align: center;
    margin-bottom: 2rem;
  }

  .ls-title {
    font-size: 2.5rem;
    color: #00bcd4;
  }

  .ls-subtitle {
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

  .example {
    margin-bottom: 1.5rem;
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