<template>
  <section class="main-body section">
    <div class="container">
      <p class="title pb-2">
        <strong>/azlilsafwan</strong>
      </p>
      <p class="subtitle">
        a <span>Web Developer</span>
      </p>
      <p class="description">
        Over the past few years, I've immersed myself in building and scaling backend software while actively tackling frontend challenges.
      </p>
      <div class="icons-section">
        <a href=""><font-awesome-icon :icon="['fab', 'github']" /></a>
        <a href=""><font-awesome-icon :icon="['fab', 'linkedin']" /></a>
        <a href=""><font-awesome-icon :icon="['fab', 'instagram']" /></a>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
  .main-body {
    padding: 8rem 26rem;
  }
  .title {
    font-size: 3rem;
  }
  .subtitle {
    font-size: 2rem;
  }
  .description {
    font-size: 1.5rem;
  }
  .icons-section {
    font-size: 2rem;
  }
</style>