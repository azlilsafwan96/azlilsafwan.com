<script setup>
import { ref } from 'vue';
const scrollToSection = (id) => {
  const element = document.getElementById(id);
  if (element) {
    element.scrollIntoView({ behavior: 'smooth' });
  }
};
const logo = ref('</.>');
</script>

<template>
  <nav 
    class="navbar" 
    role="navigation" 
    aria-label="main navigation"
  >
    <div class="navbar-brand is-flex">
      <a href="#home" class="navbar-items has-text-white has-text-weight-bold pt-4" @click.prevent="scrollToSection('home')">
        {{ logo }}
      </a>
    </div>
    <div class="navbar-end is-flex">
      <a href="#home" class="navbar-item" @click.prevent="scrollToSection('home')">
        home
      </a>
      <a href="#about" class="navbar-item" @click.prevent="scrollToSection('about')">
        about
      </a>
      <a href="#projects" class="navbar-item" @click.prevent="scrollToSection('projects')">
        projects
      </a>
    </div>
  </nav>
</template>

<style scoped>
  .navbar {
    padding: 2rem 25rem;
    margin: 0 auto;
  }
</style>