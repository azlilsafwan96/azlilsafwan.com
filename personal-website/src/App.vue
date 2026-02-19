<script setup>
import Header from './views/Header.vue';
import Footer from './views/Footer.vue';
import Main from './views/Main.vue';
</script>

<template>
  <section class="hero is-fullheight">
    <div class="hero-head">
      <Header />
    </div>
    <div class="hero-body">
      <div class="container has-text-centered">
        <Main />
      </div>
    </div>
    <div class="hero-foot">
      <Footer />
    </div>
  </section>
</template>
