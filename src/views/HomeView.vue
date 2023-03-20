<script setup>
import { onMounted } from 'vue';
import gsap from 'gsap'
import ArrowIcon from '../assets/icons/ArrowIcon.vue'
onMounted(() => {
  gsap.fromTo(".intro",{
    x:"-100%"
  },{
    x:"0",
    ease:"fade.inOut",
    duration:1.5
  })
  gsap.fromTo("#heading",{
    opacity: 0,
  },{
    opacity:1,
    delay:1,
    ease: "fade.inOut"
  })
  gsap.fromTo(".serviceBtn",{
    x: "-100%",
    opacity:0
  },{
    opacity:1,
    x:0,
    delay:2,
    ease: "bounce.out"
  })
  gsap.fromTo(".contactBtn",{
    x: "100%",
    opacity:0
  },{
    opacity:1,
    x:0,
    delay:2,
    ease: "bounce.out"
  })
})
</script>

<template>
  <main class="container">
    <div class="intro">
      <img src="../assets/IdealMark 3.png" alt="" />
      <p>Delivering our best</p>
    </div>
    <section>
      <h1 id="heading">
        One stop business solutions for <span class="highlight">Marketing</span> and
        <span class="highlight">Consultancy </span>needs.
      </h1>
      <div>
        <button class="serviceBtn">Our service <ArrowIcon /></button>
        <button class="contactBtn">Get in touch <ArrowIcon /></button>
      </div>
    </section>
  </main>
</template>

<style>
.container {
  background: #1e1eeb;
  min-height: 80vh;
}
.intro {
  display: grid;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding-top: 4rem;
  margin: auto;
  justify-items: end;
}
.intro img {
  height: 8rem;
}
.intro p {
  color: white;
  font-style: italic;
  font-size: 30px;
  padding-top: 1rem;
  margin: 0;
}
section {
  display: flex;
  align-items: center;
  flex-direction: column;
  padding-top: 5rem;
  width: 34rem;
  margin: auto;
}
section h1 {
  font-size: 32px;
  color: white;
  text-align: center;
}
.highlight {
  color: red;
  font-style: italic;
}
section > div {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
  gap: 2.5rem;
  padding-top: 2.5rem;
}
.serviceBtn {
  background: red;
  border: 1px solid red;
  color: white;
  display: flex;
  align-items: center;
  gap: 15px;
}
.contactBtn {
  background: transparent;
  border: 1px solid white;
  color: white;
  display: flex;
  align-items: center;
  gap: 15px;
}
button:hover{
  transform: scale(0.98);
}
</style>
