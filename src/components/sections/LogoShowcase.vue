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
  overflow: hidden;
  mask-image: linear-gradient(to right, transparent, black 10%, black 90%, transparent);
}

.logo-track {
  display: flex;
  gap: 80px;
  width: max-content;
  animation: scroll 14s linear infinite;
  will-change: transform;
  transform: translate3d(0,0,0);
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
    transform: translate3d(0,0,0);
  }
  to {
    transform: translate3d(-50%,0,0);
  }
}


@media (max-width: 768px) {

  .logo-track {
    gap: 30px;
    animation: scroll 13s linear infinite;
  }

  .logo img {
    height: 38px;
  }
}


.logo-section:hover .logo-track {
  animation-play-state: paused;
}
</style>