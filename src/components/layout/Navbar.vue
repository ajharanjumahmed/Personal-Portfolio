<script setup>

</script>

<template>
  <section>
    <div class="parent">
      <h1 class="logo">Ajhar</h1>
      <div class="menu">
        <a href="/">Services</a>
        <a href="/">Projects</a>
        <a href="/">Testimonials</a>
        <a href="/">Contacts</a>
      </div>
      <div class="menu-button">
        <div class="mobile-menu-icon">
          <i class="fa-solid fa-bars"></i>
        </div>
        <button>
          Resume
        </button>
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

  button{
    padding-left: 30px;
    padding-right: 30px;
    padding-top: 10px;
    padding-bottom: 10px;
    background-color: rgb(255, 255, 255);
    color: black;
    border-radius: 10px;
    transition: background-color 0.3s ease;
  }

  button:hover{
    background-color: aqua;
  }

  @media(max-width: 900px) {
    .menu{
      display: none;
    }
    .mobile-menu-icon{
      display: inline;
      padding-left: 20px;
    }
    button {
      font-size: 0.7rem;
      padding-left: 20px;
      padding-right: 20px;
      padding-top: 10px;
      padding-bottom: 10px;
      background-color: rgb(255, 255, 255);
      color: black;
      border-radius: 10px;
      transition: background-color 0.3s ease;
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
