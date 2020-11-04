<template>
  <div class="about">
    <!-- Section 1 -->
    <section class="sectionOneAbout aboutContainer grid centerContainer">
      <div class="imgDiv">
        <img src="../assets/logo.png" class="img-fluid" id="logo" />
        <p class="text-sm">Skapad med Vue cli v3</p>
      </div>
      <div class="AboutTextDiv">
        <h1 class="title-lg text-center">Varför denna hemsida?</h1>
        <p class="text-sm text-left">
          Jag byggde denna hemsida av intresse samt ett försök till bygga en
          modulär webbapp, med komponenter som kan återanvändas till andra Vue
          projekt.
        </p>
      </div>
    </section>
    <!-- Section 1 -->
    <section class="sectionTwoAbout aboutContainer grid centerContainer">
      <div class="imgDiv grid">
        <img src="../assets/img/day2.jpg" class="img-fluid" />
        <img src="../assets/img/evevning.jpg" class="img-fluid" />
        <img src="../assets/img/morning.jpg" class="img-fluid" />
        <img src="../assets/img/night.jpeg" class="img-fluid" />
        <img src="../assets/img/evevning.jpg" class="img-fluid" />
        <img src="../assets/img/morning.jpg" class="img-fluid" />
      </div>
      <div class="AboutTextDiv">
        <h1 class="title-lg text-center">Ett rutnät med bilder</h1>
        <p class="text-sm text-left padding-lg">
          Här tänker jag ha en sektion med ett bildrutnät, då många oftast har
          flera bilder på produkter eller människor.
        </p>
      </div>
    </section>
    <AppBackToTopBtn />
  </div>
</template>
<script>
import AppBackToTopBtn from "../components/AppBackToTopBtn.vue";
export default {
  components: { AppBackToTopBtn },
  data() {},
  methods: {},
};
</script>
<style>
@import "../assets/css/globalStyles.css";
@import "../assets/css/views/About.css";
</style>
