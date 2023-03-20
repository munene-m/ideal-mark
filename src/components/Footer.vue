<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <div class="container">
    <div class="contactInfo"></div>
    <div class="quickLinks">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About us</RouterLink>
        <RouterLink to="/services">Services</RouterLink>
        <RouterLink to="/contact">Contact us</RouterLink>
    </div>
    <div class="booking">
      <h1>Book with us</h1>
      <p>Book our service or consultancy in advance</p>
      <input type="email" name="" id="" />
      <button>Book now</button>
      <p>Social media</p>
    </div>
  </div>
</template>
<style scoped>
.container{
    background: #1e1eeb;
    min-height: 50vh;
    position: relative;
    top:14rem;
    display: grid;
    grid-template-columns: repeat(3,1fr);
    color:white;
}
.quickLinks{
    display: flex;
}
</style>