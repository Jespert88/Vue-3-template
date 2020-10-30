<template>
  <div class="card">
    <h1 class="title-lg text-center">{{ titleTxt }}</h1>
    <p class="text-sm">{{ paragraphTxt }}</p>
  </div>
</template>

<script>
export default {
  props: {
    titleTxt: String,
    paragraphTxt: String,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style>
@import "../assets/css/components/AppCard.css";
@import "../assets/css/globalStyles.css";
</style>