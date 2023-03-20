<script setup>
import Footer from '../components/Footer.vue'

</script>

<template>
  <div class="ceoProfile">
  <div class="ceoImg">
    <img src="../assets/WhatsApp_Image_2022-09-29_at_12.13 1.png" alt="Image of the CEO, Margaret">
    <!-- <h2>MS MARGARET KULA</h2>
    <span><p>Director and Founder</p>of IdealMark Consultant</span> -->
  </div>
  <div class="about">
    <h1 class="aboutHeader">About our CEO</h1>
    <p>Margaret holds a Bachelor’s degree in Marketing from the Management University of Africa and a Diploma in Public Relations,  From the Kenya Institute of Management. Margaret won the Best Student Award country wide from the Kenya Institute of Management, Kenya.</p>
      <br><p>She has over 10 years of experience in Marketing and Consultancy in various Industries.
    </p>
    <h2 class="aboutContacts">Contacts</h2>
    <p>+254722928160</p><p>Idealmarkconsultants@gmail.com</p>
  </div>
  </div>
  <div class="ceoTitle">
    <div>
      <h2>MS MARGARET KULA</h2>
    <h3><span class="highlight">Director and Founder</span> of IdealMark Consultant</h3>
    </div>
    <div>
      <img src="../assets/WhatsApp_Image_2023-02-21_at_03.39 1.png" alt="">
    </div>
  </div>
  <div class="clients">
    <h1>Our clients</h1>
    <div class="client">
      <div>
        <h3>UNIVERSAL FORCES INDUSTRIES</h3>
        <h4>Country - India</h4>
        <p>2016</p>
      </div>
      <div>
        <h3>PROCIENT ENGINEERING</h3>
        <h4>Country - India</h4>
        <p>2017 upto date</p>
      </div>
      <div>
        <h3>INDO AFRICA TRADE EXPO-QUICKMART</h3>
        <h4>Country - India</h4>
        <p>2018</p>
      </div>
      <div>
        <h3>BOSCO INDIA LTD</h3>
        <h4>Country - India</h4>
        <p>2019</p>
      </div>
      <div>
        <h3>A.S & SONS</h3>
        <h4>Country - India</h4>
        <p>2020</p>
      </div>
      <div>
        <h3>SHREENATHJI HYDRAULICS LTD</h3>
        <h4>Country - India</h4>
        <p>2022</p>
      </div>
    </div>
  </div>
  <Footer />
</template>

<style>
.ceoProfile{
  display: grid;
    grid-template-columns: repeat(2,1fr);
    margin: 1rem 2rem 1rem 6rem;
}
.ceoImg{
  display: flex;
    flex-direction: column;
    align-items: flex-start;
}
.ceoImg img{
  width:14rem;
}
.ceoTitle{
  display: grid;
    grid-template-columns: 2fr 1fr;
    align-items: center;
    margin: 1rem 1rem 1rem 6rem;
    position: absolute;
    top: 25rem;
}
.ceoTitle img{
  width:70%;
}
.highlight{
  color: #09BF05
}
  .about {
    display: flex;
    align-items: flex-start;
    justify-content: center;
    flex-direction: column;
    width: 50vw;
    margin: auto;
  }
  /* .about h1, h2{
    text-align: center;
    color: blue;
    text-decoration: underline;
  } */
  .aboutHeader, .aboutContacts{
    text-align: center;
    color: blue;
    text-decoration: underline;
  }
  .clients{
    position: relative;
    top: 14rem;
    background-color: #ccc;
    padding: 3rem;
  }
  .clients h1{
    color: #060670;
    text-decoration: underline;
  }
  .client{
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    align-items: end;
    justify-items: center;
  }
</style>
