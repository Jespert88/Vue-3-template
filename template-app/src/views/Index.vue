<template>
  <div class="pageContainer">
    <!-- Section 1 -->
    <section class="sectionOne">
      <div class="sectionOne grid">
        <div class="infoDiv">
          <h1 class="title-lg-white text-center">Info sektion</h1>
          <p class="text-sm-white">
            Denna sektionen kan innehålla kort information om t ex en eller
            flera produkter eller om ett företags huvudmål.
          </p>

          <a href="">Läs mer</a>
        </div>
        <AppCard
          v-bind:titleTxt="titleTxt"
          v-bind:paragraphTxt="paragraphTxt"
        />
      </div>
    </section>

    <!-- Section 2 -->
    <section class="sectionTwo container grid padding-lg">
      <div class="containerLeft padding-lg">
        <h1 class="title-lg">Vad är Lorem Ipsum?</h1>
        <p class="text-sm">
          Lorem Ipsum är en utfyllnadstext från tryck- och förlagsindustrin.
          Lorem ipsum har varit standard ända sedan 1500-talet, när en okänd
          boksättare tog att antal bokstäver och blandade dem för att göra ett
          provexemplar av en bok. Lorem ipsum har inte bara överlevt fem
          århundraden, utan även övergången till elektronisk typografi utan
          större förändringar. Det blev allmänt känt på 1960-talet i samband med
          lanseringen av Letraset-ark med avsnitt av Lorem Ipsum, och senare med
          mjukvaror som Aldus PageMaker.
        </p>
      </div>
      <div class="containerRight">
        <AppCard
          v-bind:titleTxt="titleTxt"
          v-bind:paragraphTxt="paragraphTxt"
        />
        <AppCard
          v-bind:titleTxt="titleTxt"
          v-bind:paragraphTxt="paragraphTxt"
        />
      </div>
    </section>
    <AppBackToTopBtn />
  </div>
</template>

<script>
import AppCard from "../components/AppCard.vue";
import AppBackToTopBtn from "../components/AppBackToTopBtn.vue";
export default {
  name: "Index",
  components: {
    AppCard,
    AppBackToTopBtn,
  },
  data() {
    return {
      titleTxt: "Kort komponent",
      paragraphTxt:
        "Både titeln och texten är data som modifieras i index.vue och tas emot i respektive komponent via props objektet, vilket gör det möjligt att modifiera denna komponent med olika innehåll flera gånger. ",
      imgSrc: "../assets/logo.png",
    };
  },
};
</script>

<style>
@import "../assets/css/views/Index.css";
@import "../assets/css/globalStyles.css";
</style>