<script setup>
import Java from '/src/assets/logos/Frame 5.png';
import C from '/src/assets/logos/image 7.png';
import cplus from '/src/assets/logos/image 8.png';
import python from '/src/assets/logos/image 9.png';
import htmlCss from '/src/assets/logos/image 10.png';
</script>

<template>
  <section>
    <div class="parent">
      <div class="heading">
        <h2>Tools & Technologies</h2>
      </div>
      <div class="logos">
        <div class="logo-card">
          <div class="logo">
            <img :src="C" alt="company logo" />
          </div>
        </div>
        <div class="logo-card">
          <div class="logo">
            <img :src="cplus" alt="company logo" />
          </div>
        </div>
        <div class="logo-card">
          <div class="logo">
            <img :src="python" alt="company logo" />
          </div>
        </div>
        <div class="logo-card">
          <div class="logo">
            <img :src="Java" alt="company logo" />
          </div>
        </div>
        <div class="logo-card">
          <div class="logo">
            <img :src="htmlCss" alt="company logo" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Iceland&display=swap');

section {
  padding: 0 25px;
  margin-bottom: 100px;
}

.parent {
  max-width: 1200px;
  margin: 0 auto;
}

.heading {
  margin-top: 80px;
}

.heading h2 {
  font-family: "Iceland", sans-serif;
  font-size: clamp(2.5rem, 6vw, 50px);
  font-weight: 400;
  text-align: center;
}


.logos {
  display: flex;
  flex-wrap: wrap;      
  justify-content: center;
  gap: 30px;            
  margin-top: 50px;
}


.logo-card {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 140px;
  height: 120px;
  padding: 20px;
  border: 1px solid #ffffff;
  background-color: #2e2e2e41;
  border-radius: 10px;
  transition: 0.3s ease;
}

.logo-card:hover {
  transform: translateY(-5px);
  border-color: #00ffff;
}


.logo img {
  max-width: 100%;
  max-height: 60px;
  object-fit: contain;
}


@media (max-width: 768px) {
  .logo-card {
    width: 100px;
    height: 80px;
  }
  .logo img {
    max-width: 100%;
    max-height: 50px;
    object-fit: contain;
  }
}


@media (max-width: 480px) {
  .heading h2 {
    font-size: 2rem;
  }

  .logo-card {
    width: 100px;
    height: 90px;
  }

  .logos {
    gap: 20px;
  }
}
</style>
