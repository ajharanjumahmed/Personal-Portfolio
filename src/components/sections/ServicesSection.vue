<script setup>
  import UiUx from '/src/assets/uiux.png';
  import WordPress from '/src/assets/wordpress.png';
  import PHP from '/src/assets/php.jpg';
  import Branding from '/src/assets/branding.jpg';
  import { ref } from 'vue';

  let selectedSection = ref(2);

  function changeSection(value)
  {
    selectedSection.value = value;
  }
</script>

<template>
  <section>
    <div class="parent">
      <div class="child1">
        <div class="button">
          <p>What I Do</p>
        </div>
      </div>
      <div class="child2">
        <div class="links">
          <button @click="changeSection(1)" :class="{ active: selectedSection === 1 }">UI/UX Design</button> 
          <button @click="changeSection(2)" :class="{ active: selectedSection === 2 }">WordPres Website</button>
          <button @click="changeSection(3)" :class="{ active: selectedSection === 3 }">PHP Development</button>
          <button @click="changeSection(4)" :class="{ active: selectedSection === 4 }">Branding</button>
        </div>
        <div class="card" v-if="selectedSection==1">
          <div class="image">
            <img :src="UiUx" alt="ui-ux image">
          </div>
          <div class="divider"></div>
          <div class="text">
            <h2>UI/UX Design</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi </p>
          </div>
        </div>
        <div class="card" v-if="selectedSection==2">
          <div class="image">
            <img :src="WordPress" alt="wordpress image">
          </div>
          <div class="divider"></div>
          <div class="text">
            <h2>Wordpress Website Development</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi </p>
          </div>
        </div>
        <div class="card" v-if="selectedSection==3">
          <div class="image">
            <img :src="PHP" alt="PHP image">
          </div>
          <div class="divider"></div>
          <div class="text">
            <h2>PHP Website Development</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi </p>
          </div>
        </div>
        <div class="card" v-if="selectedSection==4">
          <div class="image">
            <img :src="Branding" alt="branding image">
          </div>
          <div class="divider"></div>
          <div class="text">
            <h2>Branding</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi </p>
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
  margin-bottom: 120px;
  padding: 0 24px;
}


.parent {
  max-width: 1200px;
  margin: 0 auto;
}


.button {
  padding: 10px 30px;
  border: 1px solid white;
  width: fit-content;
  border-radius: 500px;
  background-color: #2e2e2e41;
}


.links {
  font-family: "Iceland", sans-serif;
  font-size: clamp(2rem, 6vw, 4rem);
  font-weight: 400;
  margin-top: 60px;
}

.links button{
  display: flex;
  flex-direction: column;
  text-align: left;
  background: transparent;
  border: none;
  color: rgb(88, 88, 88);
  font-family: "Iceland", sans-serif;
  font-size: inherit;
  cursor: pointer;
  transition: 0.3s ease;
}


.links button:hover {
  color: #ffffff;
}

.links button.active {
  color: #ffffff;
  border-bottom: 2px solid #ffffff;
}

.child2 {
  display: flex;
  justify-content: space-between;
  gap: 80px;
}


.card {
  margin-top: 60px;
  width: 50%;
  max-height: 500px;
  border-radius: 12px;
}


.image img{
  max-height: 300px;
  width: 100%;
  object-fit: cover;

}

.divider {
  height: 1px;
  background-color: white;
  margin-top: 30px;
  margin-bottom: 10px;
}

.card h2{
  font-size: clamp(2rem, 6vw, 20px);
  font-weight: 400;
  margin-bottom: 10px;
}

@media (max-width: 992px) {
  .child2 {
    gap: 50px;
  }

  .card {
    width: 45%;
  }
}

@media (max-width: 768px) {

  .child2 {
    flex-direction: column;
    gap: 40px;
  }

  .links {
    font-size: 2.5rem;
    margin-top: 30px;
  }

  .card {
    width: 100%;             
    margin-top: 20px;
  }

  .button p{
    font-size: 10px;
  }

}

</style>
