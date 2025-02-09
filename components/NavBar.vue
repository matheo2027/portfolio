<template>
  <nav class="navbar">
    <div class="navbar-container">
      <NuxtLink to="/" class="navbar-logo">
        <span class="logo-text">Mon Portfolio</span>
      </NuxtLink>

      <div class="navbar-right">
        <ul class="navbar-menu">
          <li><NuxtLink to="/" class="navbar-link"><i class="fas fa-home"></i> Accueil</NuxtLink></li>
          <li><NuxtLink to="/about" class="navbar-link"><i class="fas fa-user"></i> À propos</NuxtLink></li>
          <li class="dropdown">
            <a href="#" class="navbar-link"><i class="fas fa-folder"></i> Projets <i class="fas fa-chevron-down"></i></a>
            <ul class="dropdown-menu">
              <li><NuxtLink to="/projets/web" class="dropdown-link">Projet Web</NuxtLink></li>
              <li><NuxtLink to="/projets/graphique" class="dropdown-link">Projet graphique</NuxtLink></li>
              <li><NuxtLink to="/projets/ls" class="dropdown-link">My_ls</NuxtLink></li>
            </ul>
          </li>
          <li><NuxtLink to="/contact" class="navbar-link"><i class="fas fa-envelope"></i> Contact</NuxtLink></li>
        </ul>

        <button class="theme-toggle" @click="toggleTheme">
          <i :class="themeIcon"></i>
        </button>
      </div>

      <button class="navbar-toggle" @click="toggleMenu">
        <i class="fas fa-bars"></i>
      </button>
    </div>

    <ul :class="['navbar-menu-mobile', { 'active': isMenuOpen }]">
      <li><NuxtLink to="/" class="navbar-link"><i class="fas fa-home"></i> Accueil</NuxtLink></li>
      <li><NuxtLink to="/about" class="navbar-link"><i class="fas fa-user"></i> À propos</NuxtLink></li>
      <li class="dropdown">
        <a href="#" class="navbar-link" @click="toggleDropdown"><i class="fas fa-folder"></i> Projets <i class="fas fa-chevron-down"></i></a>
        <ul :class="['dropdown-menu-mobile', { 'active': isDropdownOpen }]">
          <li><NuxtLink to="/projets/web" class="dropdown-link">Projet Web</NuxtLink></li>
          <li><NuxtLink to="/projets/graphique" class="dropdown-link">Projet graphique</NuxtLink></li>
          <li><NuxtLink to="/projets/ls" class="dropdown-link">My_ls</NuxtLink></li>
        </ul>
      </li>
      <li><NuxtLink to="/contact" class="navbar-link"><i class="fas fa-envelope"></i> Contact</NuxtLink></li>
    </ul>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

const isDropdownOpen = ref(false);
const toggleDropdown = () => {
  isDropdownOpen.value = !isDropdownOpen.value;
};

const isDarkMode = ref(false);
const themeIcon = ref('fas fa-moon');

const toggleTheme = () => {
  isDarkMode.value = !isDarkMode.value;
  themeIcon.value = isDarkMode.value ? 'fas fa-sun' : 'fas fa-moon';
  document.body.classList.toggle('dark-theme', isDarkMode.value);
};
</script>

<style scoped>
.navbar {
  background: linear-gradient(135deg, #1a1a1a, #333);
  padding: 1rem 2%;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
}

.navbar-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  width: 100%;
  margin: 0 auto;
  padding: 0 2%;
}

.navbar-logo {
  text-decoration: none;
}

.logo-text {
  color: #fff;
  font-size: 1.5rem;
  font-weight: bold;
  background: linear-gradient(45deg, #00bcd4, #0097a7);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  transition: transform 0.3s ease;
}

.logo-text:hover {
  transform: scale(1.05);
}

.navbar-right {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  flex-wrap: wrap;
}

.navbar-menu {
  list-style: none;
  display: flex;
  gap: 1.5rem;
  margin: 0;
  padding: 0;
}

.navbar-menu-mobile {
  display: none;
  list-style: none;
  flex-direction: column;
  background: #1a1a1a;
  position: absolute;
  top: 100%;
  left: 0;
  width: 100%;
  padding: 1rem;
}

.navbar-menu-mobile.active {
  display: flex;
}

.navbar-link {
  color: #fff;
  text-decoration: none;
  font-size: 1rem;
  position: relative;
  padding: 0.5rem 0;
  transition: color 0.3s ease;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.navbar-link::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: linear-gradient(45deg, #00bcd4, #0097a7);
  transform: scaleX(0);
  transform-origin: right;
  transition: transform 0.3s ease;
}

.navbar-link:hover::after {
  transform: scaleX(1);
  transform-origin: left;
}

.navbar-link:hover {
  color: #00bcd4;
}

.nuxt-link-exact-active {
  color: #00bcd4;
  font-weight: bold;
}

.nuxt-link-exact-active::after {
  transform: scaleX(1);
}

.dropdown {
  position: relative;
}

.dropdown-menu {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background: #1a1a1a;
  list-style: none;
  padding: 0.5rem 0;
  border-radius: 4px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.dropdown:hover .dropdown-menu {
  display: block;
}

.dropdown-menu-mobile {
  display: none;
  list-style: none;
  padding-left: 1rem;
}

.dropdown-menu-mobile.active {
  display: block;
}

.dropdown-link {
  color: #fff;
  text-decoration: none;
  padding: 0.5rem 1rem;
  display: block;
  transition: background 0.3s ease;
}

.dropdown-link:hover {
  background: #333;
}

.theme-toggle {
  background: none;
  border: none;
  color: #fff;
  font-size: 1.2rem;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.theme-toggle:hover {
  transform: scale(1.1);
}

.navbar-toggle {
  display: none;
  background: none;
  border: none;
  color: #fff;
  font-size: 1.5rem;
  cursor: pointer;
}

@media (max-width: 768px) {
  .navbar-menu {
    display: none;
  }

  .navbar-toggle {
    display: block;
  }

  .navbar-menu-mobile {
    display: none;
  }

  .navbar-menu-mobile.active {
    display: flex;
  }

  .navbar-right {
    gap: 1rem;
  }
}
</style>