<script setup>
import logo1 from '/src/assets/logos/logo1.png';
import logo2 from '/src/assets/logos/lobuk-logo.png';
import logo3 from '/src/assets/logos/IASDLE-White-Logo.png';
import logo4 from '/src/assets/logos/nextstop-logo-transparent-1.png';


const logos = [logo1, logo2, logo3, logo4, logo1, logo2, logo3, logo4]
</script>

<template>
  <section class="logo-section">
    <div class="text">
      <h1>Trusted By Top Companies</h1>
    </div>
    <div class="logo-wrapper">
      <div class="logo-track">
       
        <div class="logo" v-for="(logo, index) in logos" :key="'first'+index">
          <img :src="logo" alt="company logo" />
        </div>

        
        <div class="logo" v-for="(logo, index) in logos" :key="'second'+index">
          <img :src="logo" alt="company logo" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>

.text{
  text-align: center;
  padding-bottom: 50px;
  font-size: clamp(1.2rem, 6vw, 1rem);

}

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


@keyframes scroll {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-50%);
  }
}


@media (max-width: 768px) {
  .logo-track {
    gap: 40px;
    animation-duration: 5s;
  }

  .logo img {
    height: 40px;
  }
}


.logo-section:hover .logo-track {
  animation-play-state: paused;
}
</style>