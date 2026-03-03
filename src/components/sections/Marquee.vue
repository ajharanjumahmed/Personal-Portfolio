<script setup>

</script>

<template>
  <section class="marquee">
    <div class="marquee__track">
      
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      

      
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
      <span class="marquee__item">Have A Project?</span>
      <span class="marquee__item">Let's Get Started →</span>
    </div>
  </section>
</template>

<style scoped>
  * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #ffffff;
      font-family: 'Inter', system-ui, -apple-system, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }

    
    .marquee {
      width: 100%;
      overflow: hidden;
      background: #ffffff;
      padding: 1rem 0;
    }

    
    .marquee__track {
      display: flex;
      gap: 2rem;
      width: fit-content;
      animation: scroll 20s linear infinite;
    }

    
    .marquee__item {
      flex: 0 0 auto;
      padding: 0.75rem 2rem;
      border-radius: 100px;
      font-size: 1.25rem;
      font-weight: 500;
      color: #0f172a;
      white-space: nowrap;
      transition: all 0.2s ease;
    }

    
    @keyframes scroll {
      0% {
        transform: translateX(-50%);
      }
      100% {
        transform: translateX(0);
      }
    }

    
    @media (max-width: 640px) {
      .marquee__item {
        font-size: 1rem;
        padding: 0.6rem 1.5rem;
      }
      .marquee__track {
        gap: 1.5rem;
      }
    }
</style>
