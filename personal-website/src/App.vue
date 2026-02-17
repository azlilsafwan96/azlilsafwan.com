<script setup>
import Header from './views/Header.vue';
import Footer from './views/Footer.vue';
</script>

<template>
  <div class="site-container">
    <Header />
    <main id="main">
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<style scoped>
.site-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}
main {
  flex-grow: 1;
}
</style>
