<script setup>
import ignitelab from '/src/assets/ignitelab.png';
import pacmanGame from '/src/assets/pacmanGame.png';
import turfManagementSystem from '/src/assets/turfManagementSystem.png';
import iasdle from '/src/assets/iasdle.png';
</script>

<template>
  <section id="Projects">
    <div class="parent">
      <div class="button">
        <p>Projects</p>
      </div>
      <div class="heading">
        <h2>Creative & Code</h2>
        <h2 class="SecondLine">Projects I've Built</h2>
      </div>
      <div class="project-cards">
        <div class="card">

          <div class="card-image">
            <img :src="ignitelab" alt="Project Image">
          </div>

          <div class="card-content">

            <div class="tags">
              <span>UI/UX Design</span>
              <span>Wordpress Development</span>
            </div>

            <h2>Ignitelab Website Design & Development</h2>

            <p>
              Ignitelab is a video editing agency specialized in editing YouTube videos. I designed and created a clean and professional website for them using WordPress.
            </p>

            <div class="buttons">
              <a href="https://ignitelabbd.com/" class="btn">Live Website</a>
            </div>

          </div>
        </div>

        <div class="card">

          <div class="card-image">
            <img :src="turfManagementSystem" alt="Project Image">
          </div>

          <div class="card-content">

            <div class="tags">
              <span>UI/UX Design</span>
              <span>PHP Development</span>
            </div>

            <h2>Book My Turf - A Turf Management System</h2>

            <p>
              A comprehensive Turf Management System built to simplify indoor ground bookings. I developed a clean, user-friendly web application that enables efficiently book and manage grounds, time slots, bookings, and payments.
            </p>

            <div class="buttons">
              <a href="https://github.com/ajharanjumahmed/Book-My-Turf" class="btn">Github</a>
            </div>

          </div>
        </div>
        <div class="card">

          <div class="card-image">
            <img :src="pacmanGame" alt="Project Image">
          </div>

          <div class="card-content">

            <div class="tags">
              <span>Java</span>
              <span>Game Development</span>
            </div>

            <h2>Pacman Game Development</h2>

            <p>
              This project implements the fundamental mechanics of Pac-Man: navigating a maze, collecting all pellets, and avoiding ghosts. Built solely in Java using the Swing toolkit
            </p>

            <div class="buttons">
              <a href="https://github.com/ajharanjumahmed/Pacman-Game-using-Java" class="btn">Github</a>
            </div>

          </div>
        </div>

        <div class="card">

          <div class="card-image">
            <img :src="iasdle" alt="Project Image">
          </div>

          <div class="card-content">

            <div class="tags">
              <span>UI/UX Design</span>
              <span>Wordpress Development</span>
            </div>

            <h2>IASDLE Website Design & Development</h2>

            <p>
              IASDLE is a modern, responsive organizational website developed to showcase its mission and activities with a clean design, structured content, and smooth user experience.
            </p>

            <div class="buttons">
              <a href="https://iasdle.com/" class="btn">Live Website</a>
            </div>

          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Iceland&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap');

section {
  margin-bottom: 80px;
  padding: 0 20px;
}


.parent {
  max-width: 1200px;
  margin: 0 auto;
}


.button {
  padding: 8px 22px;
  border: 1px solid white;
  width: fit-content;
  border-radius: 500px;
  background-color: #2e2e2e41;
  font-size: 14px;
}


.heading {
  padding-top: 20px;
  font-family: "Iceland", sans-serif;
  font-size: clamp(3rem, 7vw, 4rem);
  font-weight: 400;
}

.SecondLine {
  margin-top: -25px;
}


.project-cards {
  display: grid;
  grid-template-columns: 1fr;
  gap: 30px;
  padding-top: 80px;
}


.card {
  width: 100%;
  border-radius: 12px;
  overflow: hidden;
  background: #121212;
  box-shadow: 0 0 0 1px rgba(255, 255, 255, 0.185);
  transition: all 0.4s ease;
  cursor: pointer;
}


.card:hover {
  transform: translateY(-12px);
  box-shadow: 0 15px 40px rgba(0, 255, 255, 0.15);
}


.card-image {
  overflow: hidden;
}

.card-image img {
  width: 100%;
  height: 240px;
  object-fit: cover;
  display: block;
  transition: transform 0.5s ease;
}


.card:hover .card-image img {
  transform: scale(1.08);
}


.card-content {
  padding: 20px;
}


.tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-bottom: 15px;
}

.tags span {
  background: #252525;
  padding: 6px 10px;
  font-size: 12px;
  border-radius: 4px;
  color: #d0d0d0;
}

.card-content h2 {
  font-family: "Iceland", sans-serif;
  font-size: 24px;
  font-weight: 400;
  color: white;
  margin-bottom: 12px;
}

.card-content p {
  font-size: 14px;
  line-height: 1.6;
  color: #a0a0a0;
  margin-bottom: 20px;
}

.buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}

.btn {
  padding: 8px 16px;
  border: 1px solid white;
  color: white;
  text-decoration: none;
  font-size: 13px;
  border-radius: 4px;
  transition: all 0.3s ease;
}

.btn:hover {
  background: cyan;
  color: black;
  transform: translateY(-3px);
}


@media (min-width: 640px) {
  .project-cards {
    grid-template-columns: repeat(2, 1fr);
  }

  .card-image img {
    height: 260px;
  }
}


@media (min-width: 1024px) {
  .project-cards {
    grid-template-columns: repeat(2, 1fr);
    gap: 50px;
  }

  .card-image img {
    height: 300px;
  }

  .card-content h2 {
    font-size: 28px;
  }
}
</style>
