<template>
  <div class="bg-white px-6 py-24 sm:py-5 lg:px-8">
    <div class="mx-auto max-w-2xl text-center">
      <p class="text-base font-semibold leading-7 text-indigo-600">Portfolio</p>
      <h2 class="mt-2 text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">Clément HAUSKNECHT</h2>
      <img class="mx-auto mt-6 h-60 w-60 rounded-full object-cover" src="./img/face.png" alt="Clément HAUSKNECHT">
      <p class="mt-6 text-lg leading-8 text-gray-600">Welcome to my portfolio! Discover my professional experience, skills and achievements.</p>
      <div class="mt-20 mb-1 flex justify-center">
        <div class="arrow-container" id="scroll-arrow">
          <div class="arrow"></div>
        </div>
      </div>
      <p class="mt-20 text-2xl font-semibold leading-7 text-indigo-600 text-center">My qualifications</p>
    </div>
  </div>
</template>

<style scoped>
.arrow-container {
  width: 24px;
  height: 24px;
}

.arrow {
  width: 0;
  height: 0;
  border-left: 12px solid transparent;
  border-right: 12px solid transparent;
  border-top: 24px solid #4f46e5; 
  animation: bounce 2s infinite;
  transition: opacity 0.5s ease-out; /* Transition de base pour l'opacité */
  opacity: 1;
}
</style>

<script>
export default {
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
    this.handleScroll(); // Vérifiez la position initiale lors du montage
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const arrow = document.getElementById('scroll-arrow').querySelector('.arrow');
      const scrollPosition = window.scrollY;
      const fadeStart = 0; // Point de départ du défilement où la flèche commence à disparaître
      const fadeEnd = 300; // Point de défilement où la flèche devient complètement invisible
      
      if (scrollPosition > fadeEnd) {
        arrow.style.opacity = 0;
      } else if (scrollPosition < fadeStart) {
        arrow.style.opacity = 1;
      } else {
        // Calcule l'opacité en fonction de la position de défilement
        arrow.style.opacity = 1 - (scrollPosition - fadeStart) / (fadeEnd - fadeStart);
      }
    }
  }
}
</script>
