<template>
  <div class="pageContainer">
    <section class="infoSection">
      <div class="infoSection grid">
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
  </div>
</template>

<script>
import AppCard from "../components/AppCard.vue";
export default {
  name: "Index",
  components: {
    AppCard,
  },
  data() {
    return {
      titleTxt: "Kort komponent",
      paragraphTxt:
        "Både titeln och texten är data som modifieras i index.vue och tas emot i respektive komponent via props objektet, vilket gör det möjligt att modifiera denna komponent med olika innehåll flera gånger. ",
    };
  },
};
</script>

<style>
@import "../assets/css/views/index.css";
@import "../assets/css/globalStyles.css";
</style>