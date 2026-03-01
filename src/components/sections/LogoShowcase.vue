<script setup>
import logo1 from '/src/assets/logos/logo1.png';
const logos = [logo1, logo1, logo1, logo1, logo1]
</script>

<template>
  <section class="logo-section">
    <div class="logo-wrapper">
      <div class="logo-track">
        <!-- First Set -->
        <div class="logo" v-for="(logo, index) in logos" :key="'first'+index">
          <img :src="logo" alt="company logo" />
        </div>

        <!-- Duplicate Set (for seamless loop) -->
        <div class="logo" v-for="(logo, index) in logos" :key="'second'+index">
          <img :src="logo" alt="company logo" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.logo-section {
  width: 100%;
  overflow: hidden;
  padding: 40px 0;
  background: #1D1D1D;
}

.logo-wrapper {
  display: flex;
}

.logo-track {
  display: flex;
  gap: 100px;
  animation: scroll 15s linear infinite;
}

.logo {
  flex-shrink: 0;
}

.logo img {
  height: 50px;
  width: auto;
  object-fit: contain;
  filter: grayscale(100%);
  opacity: 0.7;
  transition: 0.3s ease;
}

.logo img:hover {
  filter: grayscale(0%);
  opacity: 1;
}

/* Animation */
@keyframes scroll {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-50%);
  }
}

/* Responsive */
@media (max-width: 768px) {
  .logo-track {
    gap: 40px;
    animation-duration: 4s;
  }

  .logo img {
    height: 40px;
  }
}

/* Pause on hover */
.logo-section:hover .logo-track {
  animation-play-state: paused;
}
</style>