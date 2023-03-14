<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <div class="secondaryNav">
        <div class="socials">
          <i><img src="./assets/whatsapp.png" alt="" /></i>
          <i><img src="./assets/twitter.png" alt="" /></i>
          <i><img src="./assets/Vector7.png" alt="" /></i>
          <i><img src="./assets/facebook.png" alt="" /></i>
          <i><img src="./assets/linkedin.png" alt="" /></i>
        </div>
        <div class="contacts">
          <div>
            <p>Phone number</p>
            <p>+254 722928160</p>
          </div>
          <div>
            <p>Free consultancy/Enquiries:</p>
            <p>ceoidealmarkconsultants@gmail.com</p>
          </div>
        </div>
      </div>
      <nav>
        <div class="navIcon">
          <img src="./assets/idealMark 2.png" alt="">
        </div>
        <div class="navItems">
          <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About us</RouterLink>
        <RouterLink to="/services">Services</RouterLink>
        <RouterLink to="/contact">Contact us</RouterLink>
        </div>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
}
.secondaryNav {
  background: #1e1eeb;
  display: flex;
  justify-content: space-between;
  padding: 2rem 0.8rem 0.5rem 0.8rem;
}
.socials {
  display: flex;
  align-items: flex-end;
  gap:10px;
}
.socials i img {
  height: 13px;
}
.contacts {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-items: center;
}
.contacts > div > p {
  color: white;
  margin: 0;
  font-size: 12px;
}

nav {
  width: 100%;
  max-width: -webkit-fill-available;
  font-size: 12px;
  text-align: center;
  padding: 1rem 0.8rem;
  display: flex;
    justify-content: space-between;
    background: #1e1eeb;
    border-top: 1px solid white;
    border-bottom: 1px solid white;
}
nav a {
  text-decoration: none;
  color:white;
  transition: .3s ease-in;
}
nav a:hover{
  transform: scale(1.2);
}
.navIcon img{
  height:35px;
}
.navItems{
  display: flex;
    align-items: center;
    gap: 3rem;
    font-size: 16px;
}

/* nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
} */
</style>
