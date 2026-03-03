<script setup>
import heroImage from '/src/assets/heroImage.png';
</script>

<template>
  <section id="Hero">
    <div class="parent">
      <div class="text">
        <div class="text-content">
          <div class="heading">
            <div class="header2">
              <h2>Ajhar</h2>
              <h2 id="n2">Anjum Ahmed</h2>
            </div>
            <p>--- programmer, ui/ux designer</p>
          </div>
          <div class="subheading">
            <p>I’m a Computer Science student, programmer, and UI/UX designer passionate about building functional,
              user-centered digital solutions. I combine clean code with intuitive design to create simple, and
              impactful
              solutions.</p>
          </div>
        </div>
      </div>
      <div class="image">
        <img :src="heroImage" alt="image">
      </div>
    </div>
  </section>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Iceland&display=swap');

*{
  margin-left: 10px;
  margin-right: 10px;
}

section {
  min-height: screen;
  display: flex;
  align-items: center;
}

.parent {
  display: flex;
  width: 100%;
}


.text,
.image {
  flex: 1;
  box-sizing: border-box;
}


.text {
  color: white;
  display: flex;
  align-items: center;
}

.heading {
  margin-bottom: 2rem;
}

.text-content {
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: clamp(20px, 6vw, 200px);
}

.text h2 {
  font-family: "Iceland", sans-serif;
  font-size: clamp(4rem, 6vw, 5rem);
  font-weight: 400;
  line-height: 1;
  margin: 0;
}

.heading p {
  font-family: "Iceland", sans-serif;
  font-size: clamp(1rem, 5vw, 34px);
  margin-top: 10px;
}

.subheading p {
  margin-top: 38px;
  font-size: clamp(0.9rem, 1.5vw, 16px);
  max-width: 500px;
  line-height: 1.6;
  color: rgba(255, 255, 255, 0.37);
}


.image {
  display: flex;
}

.image img {
  width: 100%;
  max-width: 900px;
  height: auto;
  object-fit: cover;
}


@media (max-width: 768px) {

  *{
    margin-left: 0px;
    margin-right: 0px;
  }

  .parent {
    flex-direction: column;
  }

  .text {
    text-align: center;
    justify-content: center;
  }

  .subheading p {
    margin-left: auto;
    margin-right: auto;
    margin-top: 0px;
  }
}
</style>
