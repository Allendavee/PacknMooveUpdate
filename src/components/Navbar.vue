<template>

  <header class="header">
      
    <nav class="navbar">
      <router-link :to="{ name: 'Home' }" class="nav-logo"
        ><img src="@/assets/logo.png"
      /></router-link>
      <ul class="nav-menu">
        <li class="nav-item">
          <router-link :to="{ name: 'Home' }" class="nav-link"
            >Home</router-link
          >
        </li>
        <li class="nav-item">
          <router-link :to="{ name: 'Services' }" class="nav-link"
            >Services</router-link
          >
        </li>
        <li class="nav-item">
          <router-link :to="{ name: 'About' }" class="nav-link"
            >About Us</router-link
          >
        </li>
        <li class="nav-item">
          <router-link :to="{ name: 'Contact' }" class="nav-link"
            >Contact Us</router-link
          >
        </li>
      </ul>
      <div class="hamburger" @click="mobileMenu()">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
    </nav>
  </header>
</template>

<script>


export default {
  data() {
    return {};
  },
  methods: {
    mobileMenu() {
      const hamburger = document.querySelector(".hamburger");
      const navMenu = document.querySelector(".nav-menu");

      hamburger.classList.toggle("active");
      navMenu.classList.toggle("active");
    },
    closeMenu() {
      const hamburger = document.querySelector(".hamburger");
      const navMenu = document.querySelector(".nav-menu");

      hamburger.classList.remove("active");
      navMenu.classList.remove("active");
    },
  },
};
</script>

<style lang="css" scoped>
@import url("https://fonts.googleapis.com/css2?family=Quicksand:wght@300;400;500&display=swap");

.header {
  width: 100%;
}
.navbar {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 5%;
}
.nav-logo > img {
    width: 150px;
}

.nav-menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.nav-item {
  padding: 0 16px;
  list-style-type: none;
}
.nav-menu a {
  text-decoration: none;
  font-family: "Inter", sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 19px;
  color: #616060;
  cursor: pointer;
  animation: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
}
.router-link-exact-active:nth-child(1) {
  color: #0187BA;

}
.router-link-exact-active:nth-child(2) {
  color: #0187BA;
}
.router-link-exact-active:nth-child(3) {
  color: #0187BA;
}
.router-link-exact-active:nth-child(3) {
  color: #0187BA;
}
.hamburger {
  display: none;
}
.bar {
  display: block;
  width: 25px;
  height: 3px;
  margin: 5px auto;
  animation: all 0.3s ease-in-out;
  transition: all 0.3s ease-in-out;
  background-color: #101010;
}

@media only screen and (max-width: 800px) {
  .hamburger {
    display: block;
    cursor: pointer;
  }
  .hamburger.active .bar:nth-child(2) {
    opacity: 0;
  }

  .hamburger.active .bar:nth-child(1) {
    transform: translateY(8px) rotate(45deg);
  }

  .hamburger.active .bar:nth-child(3) {
    transform: translateY(-8px) rotate(-45deg);
  }
}
</style>