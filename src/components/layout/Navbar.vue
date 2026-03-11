<script setup>
import Logo from "/src/assets/300ppi/Ajhar Logo.png";

import { ref } from 'vue';


const isMenuOpen = ref(false)


const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value
}


const closeMenu = () => {
  isMenuOpen.value = false
}
</script>

<template>
  <section>
    <div class="parent">
      <img :src="Logo" alt="ajhar logo">
      <div class="menu">
        <a href="#Services">Services</a>
        <a href="#Projects">Projects</a>
        <a href="#Testimonials">Testimonials</a>
        <a href="#Contacts">Contacts</a>
      </div>
      <div class="menu-button">
        <div class="mobile-menu-icon" @click="toggleMenu">
          <i class="fa-solid fa-bars">
          </i>
        </div>
        <div class="button">
          <a href="https://drive.google.com/file/d/1mUygGrxhNa-JyQygu0xNiMrzaxF3249p/view?usp=sharing">Resume</a>
        </div>    
      </div>
    </div>
    
    <div v-if="isMenuOpen" class="mobile-menu-overlay">
      <div class="mobile-menu-content">
        <button class="close-btn" @click="closeMenu">✕</button>
        <a href="#Services" @click="closeMenu">Services</a>
        <a href="#Projects" @click="closeMenu">Projects</a>
        <a href="#Testimonials" @click="closeMenu">Testimonials</a>
        <a href="#Contacts" @click="closeMenu">Contacts</a>
      </div>
    </div>
  </section>
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Iceland&display=swap');

  .parent{
    color: rgb(255, 255, 255);
    min-width: screen;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-left: 7rem;
    margin-right: 7rem;
    height: 4rem;
    margin-top: 1.2rem;
  }

  .parent img{
    max-height: 40px;
  }

  .logo{
    font-family: "Iceland", sans-serif;
    font-size: 3rem;
    font-weight: 400;
    font-style: normal;
  }

  .menu{
    display: flex;
    gap: 2rem;
    font-size: 1rem;
  }

  .menu a{
    transition: color 0.3s ease;
  }

  .menu a:hover{
    color: aqua;
  }

  .mobile-menu-icon{
    display: none;
  }

  .menu-button{
    display: flex;
    align-items: center;
    gap: 2rem;
  }

  .button{
    display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: #ffffff28;
  color: white;
  padding: 0.7rem 1.5rem;
  border-radius: 40px;
  font-weight: 500;
  font-size: 0.95rem;
  text-decoration: none;
  width: fit-content;
  transition: background 0.2s ease, transform 0.1s ease;
  border: 1px solid #ffffff;
  }

.button:hover{
  transform: scale(1.02);
  border: 1px solid aqua;
  }

  .mobile-menu-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.95);
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  z-index: 999;
}

.mobile-menu-content {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  text-align: center;
}

.mobile-menu-content a {
  color: white;
  font-size: 1.5rem;
  text-decoration: none;
  transition: color 0.3s ease;
}

.mobile-menu-content a:hover {
  color: aqua;
}

.close-btn {
  position: absolute;
  top: 2rem;
  right: 2rem;
  background: none;
  border: none;
  font-size: 2rem;
  color: white;
  cursor: pointer;
}

  @media(max-width: 900px) {
    .mobile-menu-overlay {
    display: flex;
  }
    .menu{
      display: none;
    }
    .mobile-menu-icon{
      display: inline;
      padding-left: 20px;
    }
    .button {
      font-size: 0.7rem;
      padding-left: 20px;
      padding-right: 20px;
      padding-top: 10px;
      padding-bottom: 10px;
      background: #ffffff28;
      color: white;
      border-radius: 10px;
      transition: background 0.2s ease, transform 0.1s ease;
      border: 1px solid #ffffff;
    }    
    .parent {
      color: rgb(255, 255, 255);
      min-width: screen;
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-left: 2rem;
      margin-right: 2rem;
      height: 4rem;
      margin-top: 1.2rem;
    }
  }
</style>
