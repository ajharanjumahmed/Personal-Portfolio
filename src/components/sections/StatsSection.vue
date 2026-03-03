<script setup>

</script>

<template>
  <section class="stats-section">
  <div class="stat-item">
    <span class="stat-number">30+</span>
    <span class="stat-label">Global Clients</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">4+</span>
    <span class="stat-label">Years Of Experience</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">4.9</span>
    <span class="stat-label">Average Rating</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">99%</span>
    <span class="stat-label">Success Rate</span>
  </div>
</section>
</template>

<style scoped>
  .stats-section {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 2rem;
  padding: 0rem 2rem;
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
  margin-bottom: 70px;
  margin-top: -50px;
}

.stat-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 2rem 1rem;
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.stat-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px rgba(0,0,0,0.1);
}

.stat-number {
  font-size: 3rem;
  font-weight: 700;
  color: #ffffff;
  line-height: 1.2;
}

.stat-label {
  font-size: 1.1rem;
  color: #ffffff44;
  text-transform: uppercase;
  letter-spacing: 0.5px;
  margin-top: 0.5rem;
}

@media (max-width: 768px) {
  .stats-section {
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
    padding: 2rem 1rem;
  }
}

@media (max-width: 480px) {
  .stats-section {
    grid-template-columns: 1fr;
  }
}
</style>
