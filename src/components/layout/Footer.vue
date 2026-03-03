<script setup>

</script>

<template>
  <footer class="footer" id="Contacts">
    <div class="footer-container">
      
      <div class="footer-col">
        <h2 class="footer-name">
          AJHAR<br>ANJUM AHMED
        </h2>
        <p class="footer-bio">
          I'm a Computer Science student, programmer, and UI/UX designer passionate about building functional, user-centered digital solutions. I combine clean code with intuitive design to create simple, and impactful solutions.
        </p>
        <a href="https://drive.google.com/file/d/1DeMh_UEBVo8RsQx-xgYHgOsh1wZkDmGB/view?usp=sharing" class="resume-btn">📄 Resume</a>
      </div>

      
      <div class="footer-col">
        <h3 class="footer-title">Contact Me</h3>
        <ul class="contact-list">
          <li>📧 ajharanjumahmed@gmail.com</li>
          <li>📞 +8801632419628</li>
          <li>📍 Chararpar, Sylhet, Bangladesh</li>
        </ul>
      </div>

      
      <div class="footer-col">
        <h3 class="footer-title">Menu</h3>
        <ul class="menu-list">
          <li><a href="#Hero">Home</a></li>
          <li><a href="#Services">Services</a></li>
          <li><a href="#Projects">Projects</a></li>
          <li><a href="#Testimonials">Testimonial</a></li>
        </ul>
      </div>
    </div>

    
    <div class="footer-bottom">
      <p>Copyright @ 2026 Ajhar Anjum Ahmed - All Rights Reserved</p>
    </div>
  </footer>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', system-ui, -apple-system, sans-serif;
  background: #f9fafc;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}


.footer {
  background: #101010;
  border-top: 1px solid #eaeef2;
  padding: 5rem 3rem 1.5rem;
  box-shadow: 0 -4px 12px rgba(0, 0, 0, 0.02);
  margin-top: auto;
}

.footer-container {
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 2fr 1.5fr 1fr;
  gap: 8rem;
  align-items: start;
}


.footer-col {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.footer-name {
  font-size: 1.8rem;
  font-weight: 600;
  line-height: 1.2;
  color: #ffffff;
  margin-bottom: 0.5rem;
}

.footer-bio {
  color: #ffffff6e;
  line-height: 1.6;
  font-size: 0.95rem;
  margin-bottom: 0.5rem;
  max-width: 450px;
}

.resume-btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: #0b1c2f;
  color: white;
  padding: 0.7rem 1.5rem;
  border-radius: 40px;
  font-weight: 500;
  font-size: 0.95rem;
  text-decoration: none;
  width: fit-content;
  transition: background 0.2s ease, transform 0.1s ease;
  border: 1px solid #1e2e42;
}

.resume-btn:hover {
  background: #1e2e42;
  transform: scale(1.02);
}

.footer-title {
  font-size: 1.2rem;
  font-weight: 600;
  color: #ffffff;
  margin-bottom: 0.75rem;
  letter-spacing: -0.01em;
}


.contact-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
}

.contact-list li {
  display: flex;
  align-items: center;
  gap: 0.6rem;
  color: #ffffffe0;
  font-size: 0.95rem;
  line-height: 1.5;
}

.contact-list li::before {
  content: "•";
  color: #ffffffe0;
  font-weight: bold;
  font-size: 1.2rem;
  line-height: 1;
}


.menu-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 0.6rem;
}

.menu-list li a {
  color: #ffffffe0;
  text-decoration: none;
  font-size: 0.95rem;
  transition: color 0.2s ease, padding-left 0.2s ease;
  display: inline-block;
}

.menu-list li a:hover {
  color: rgba(255, 255, 255, 0.425)e0;
  padding-left: 4px;
  font-weight: 500;
}


.footer-bottom {
  text-align: center;
  margin-top: 3rem;
  padding-top: 1.5rem;
  border-top: 1px solid #e0e8ee;
  color: #ffffffb0;
  font-size: 0.9rem;
}


@media (max-width: 900px) {
  .footer-container {
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }

  .footer-col:first-child {
    grid-column: span 2; 
  }
}

@media (max-width: 600px) {
  .footer-container {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .footer-col:first-child {
    grid-column: span 1;
  }

  .footer {
    padding: 2rem 1.5rem 1rem;
  }

  .footer-name {
    font-size: 1.6rem;
  }

  .footer-bottom {
    margin-top: 2rem;
  }
}
</style>
