<script setup>
import pacmanGame from '/src/assets/pacmanGame.png';
import tamara from '/src/assets/tamara.jpg';
import pinetim from '/src/assets/pinetim.jpg';
import brainharper from '/src/assets/brainharper.jpg';
import dianep from '/src/assets/dianep.jpg';
import josh from '/src/assets/josh.jpg';
</script>

<template>
  <section id="Testimonials">
    <div class="parent">
      <div class="child1">
        <div class="button">
          <p>Testimonials</p>
        </div>
        <div class="heading">
          <h2>Experiences That Speak</h2>
          <h2 id="secondHeading"> For Themselves</h2>
        </div>
      </div>
      <div class="child2">

        <div class="testimonials">
          <div class="testimonial-row row-right">
            <div class="testimonial-track">
              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pacmanGame" alt="avatar">
                  </div>
                  <div class="testimonial-name">Alberts Fotowelt</div>
                </div>
                <div class="testimonial-text">
                  I am very satisfied with the cooperation. Delivery took place in the specified time. Price/performance is great! I'm happy to have taken this path.
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="tamara" alt="avatar">
                  </div>
                  <div class="testimonial-name">Tamara Solomson</div>
                </div>
                <div class="testimonial-text">
                  Prompt responses, and delivered what I asked for!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="dianep" alt="avatar">
                  </div>
                  <div class="testimonial-name">Dianep</div>
                </div>
                <div class="testimonial-text">
                  I ordered a signature 2 different ways. ajharahmed was very responsive, completely understood my request and delivered well before the time period. Excellent!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="josh" alt="avatar">
                  </div>
                  <div class="testimonial-name">Josh Thiele</div>
                </div>
                <div class="testimonial-text">
                  Can’t complain! Really good work. Exactly what I was looking for and good price. Would recommend 5/5!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="brainharper" alt="avatar">
                  </div>
                  <div class="testimonial-name">Brian Harper</div>
                </div>
                <div class="testimonial-text">
                  Good communication and good work.
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pinetim" alt="avatar">
                  </div>
                  <div class="testimonial-name">Pine Tim</div>
                </div>
                <div class="testimonial-text"> 
                  I would highly reccomend ajharamhed, has good professionalism and works quickly!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pacmanGame" alt="avatar">
                  </div>
                  <div class="testimonial-name">Sarah Williams</div>
                </div>
                <div class="testimonial-text">
                  Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pacmanGame" alt="avatar">
                  </div>
                  <div class="testimonial-name">Michael Brown</div>
                </div>
                <div class="testimonial-text">
                  Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est
                  laborum.
                </div>
              </div>
            </div>
          </div>




          <div class="testimonial-row row-left">
            <div class="testimonial-track">
              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pacmanGame" alt="avatar">
                  </div>
                  <div class="testimonial-name">Alberts Fotowelt</div>
                </div>
                <div class="testimonial-text">
                  I am very satisfied with the cooperation. Delivery took place in the specified time. Price/performance is great! I'm happy to have taken this path.
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="tamara" alt="avatar">
                  </div>
                  <div class="testimonial-name">Tamara Solomson</div>
                </div>
                <div class="testimonial-text">
                  Prompt responses, and delivered what I asked for!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="dianep" alt="avatar">
                  </div>
                  <div class="testimonial-name">Dianep</div>
                </div>
                <div class="testimonial-text">
                  I ordered a signature 2 different ways. ajharahmed was very responsive, completely understood my request and delivered well before the time period. Excellent!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="josh" alt="avatar">
                  </div>
                  <div class="testimonial-name">Josh Thiele</div>
                </div>
                <div class="testimonial-text">
                  Can’t complain! Really good work. Exactly what I was looking for and good price. Would recommend 5/5!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="brainharper" alt="avatar">
                  </div>
                  <div class="testimonial-name">Brian Harper</div>
                </div>
                <div class="testimonial-text">
                  Good communication and good work.
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pinetim" alt="avatar">
                  </div>
                  <div class="testimonial-name">Pine Tim</div>
                </div>
                <div class="testimonial-text"> 
                  I would highly reccomend ajharamhed, has good professionalism and works quickly!
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pacmanGame" alt="avatar">
                  </div>
                  <div class="testimonial-name">Sarah Williams</div>
                </div>
                <div class="testimonial-text">
                  Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                </div>
              </div>

              <div class="testimonial-card">
                <div class="testimonial-header">
                  <div class="testimonial-avatar">
                    <img :src="pacmanGame" alt="avatar">
                  </div>
                  <div class="testimonial-name">Michael Brown</div>
                </div>
                <div class="testimonial-text">
                  Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est
                  laborum.
                </div>
              </div>
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
  margin-bottom: 0px;
}

.parent {
  display: flex;
  flex-direction: column;
}

.child1 {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 60px;
}

.button {
  padding: 10px 30px;
  border: 1px solid white;
  width: fit-content;
  border-radius: 500px;
  background-color: #2e2e2e41;
}

.heading {
  padding-top: 20px;
  font-family: "Iceland", sans-serif;
  font-size: clamp(2.5rem, 7vw, 4rem);
  font-weight: 400;
  text-align: center;
}

#secondHeading {
  margin-top: -30px;
}



.testimonials {
  overflow: hidden;
  padding: 80px 0;
}



.testimonial-row {
  overflow: hidden;
  position: relative;
  margin-bottom: 40px;
}

.testimonial-track {
  display: flex;
  gap: 40px;
  width: max-content;
  padding-top: 10px;
  padding-bottom: 10px;
}



.testimonial-card {
  flex: 0 0 350px;
  padding: 30px;
  border-radius: 12px;
  background: #111;
  box-shadow: 0 0 0 1px rgba(255, 244, 244, 0.08);
  transition: 0.3s ease;
}

.testimonial-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 15px 30px rgba(0, 255, 255, 0.15);
}



.testimonial-header {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-bottom: 15px;
}

.testimonial-avatar {
  width: 50px;
  height: 50px;
  border-radius: 100%;
  background: #ddd;
}

.testimonial-avatar img{
  width: 50px;
  height: 50px;
  border-radius: 100%;
  background: #ddd;
}

.testimonial-name {
  font-family: "Iceland", sans-serif;
  font-size: 18px;
  color: white;
}

.testimonial-text {
  color: rgba(255, 255, 255, 0.7);
  font-size: 14px;
  line-height: 1.6;
}


.row-left .testimonial-track {
  animation: scrollLeft 25s linear infinite;
}


.row-right .testimonial-track {
  animation: scrollRight 25s linear infinite;
}

@keyframes scrollLeft {
  from {
    transform: translateX(0);
  }

  to {
    transform: translateX(-50%);
  }
}

@keyframes scrollRight {
  from {
    transform: translateX(-50%);
  }

  to {
    transform: translateX(0);
  }
}


@media (max-width: 992px) {
  .testimonial-card {
    flex: 0 0 300px;
  }
}

@media (max-width: 768px) {

  .testimonials {
    padding: 50px 0;
  }

  .testimonial-track {
    gap: 20px;
  }

  .testimonial-card {
    flex: 0 0 260px;
    padding: 20px;
  }

  .testimonial-name {
    font-size: 16px;
  }

  .testimonial-text {
    font-size: 13px;
  }

  .button{
    font-size: 12px;
  }

  #secondHeading{
    padding-top: 15px;
  }


  .row-left .testimonial-track,
  .row-right .testimonial-track {
    animation-duration: 18s;
  }
}
</style>
