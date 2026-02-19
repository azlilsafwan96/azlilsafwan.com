<template>
  <div
    style="
      height: 100vh;
    "
  >
    <div
      style="
        height: 40rem;
        align-content: center;
      "
    >
      <p 
        class="title is-1" :aria-label="fullText"
      >{{ displayedText }}<span class="cursor">|</span></p>
    </div>
    <div>
      <p>
        scroll down
      </p>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const displayedText = ref('');
const fullText = '</azlilsafwan.>';

const typeText = () => {
  let i = 0;
  const speed = 90;

  const type = () => {
    if (i < fullText.length) {
      displayedText.value += fullText.charAt(i);
      i++;
      setTimeout(type, speed);
    }
  };

  type();
};

onMounted(() => {
  typeText();
});
</script>

<style scoped>
.cursor {
  animation: blink 1s step-end infinite;
}

@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}
</style>