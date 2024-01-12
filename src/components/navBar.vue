<script setup>
import { ref } from 'vue';

const isMenuOpen = ref(false);

const toggleMenu = () => {
  console.log('click me') 
    isMenuOpen.value = !isMenuOpen.value;
}

</script>

<template>
  <header>
    <div class="logo">
        <img src="https://res.cloudinary.com/dqrykh6qy/image/upload/v1704982751/victoria_logo_aaysca.png" alt="logo">
    </div>
    <nav class="links">
        <RouterLink active-class="active" to="/">Home</RouterLink>
        <RouterLink to="">About</RouterLink>
    </nav> 
    <button class="btn">Get my resume</button>
    <!-- <div class="hamburger-menu" @click="toggleMenu"> -->
        <!-- <span>&#9776;</span> -->
    <!-- </div> -->
  </header>
  <!-- <nav :class="{'show-menu': isMenuOpen}">
        <RouterLink active-class="active" to="/">Home</RouterLink>
        <RouterLink to="">About</RouterLink>
        <button>Get start</button> -->
  <!-- </nav>    -->
</template>

<style scoped>
header {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  background: white;
  padding: 20px;
  text-transform: uppercase;
}

/* .logo {
 
} */

 .logo img {
  max-width: 200px; 
}


nav {
  display: flex;
  /* align-items: center; */
}

nav a {
  font-size: 1.2rem;
  font-weight: 600;
  text-decoration: none;
  color: #333;
  margin: 20px;
  transition: color 1.3s ease-in-out;
}

nav a:hover {
  color: #007bff; 
}

a.active {
  color: #007bff;
}

nav.show-menu {
display: flex;
flex-direction: column;
background: white;
text-transform: uppercase;
}

nav.show-menu  {
  display: none;
  text-align: left;
  padding: 10px;
}

.btn {
  /* margin: 15px ; */
  padding: 15px 20px;
  border: 2px solid #000;
  background: #ffffff;
  font-size: 18px;
  font-weight: 600;
  text-transform: uppercase;
  cursor: pointer;
  color: rgb(29, 27, 27);
  box-shadow: 4px 5px 0px rgba(0, 0, 0, 0.99);
}

.btn:hover {
  box-shadow: 0 0 0 rgba(0, 0, 0, 0.00);
}

.hamburger-menu {
  color: rgba(41, 40, 40);
  cursor: pointer;
  font-size: 25px;
  font-weight: 600;
  display: none;
}


/* media query */
@media (max-width: 768px){
  header {
    flex-direction: row;
    justify-content: space-evenly;
    /* align-items: flex-start; */
  }

  nav.links {
    display: none;
  }

  nav.show-menu {
    display: block;
  }

  .hamburger-menu {
    display: block;
  }

  .btn {
    display: block;
    padding: 10px;
    font-size: 10px;
  }

  .logo img {
    width: 100px;
  }
 
}

@media (max-width: 320px) {
  header {
    /* flex-direction: row;
    justify-content: space-between;
    align-items: flex-start; */
  }
}
</style>

