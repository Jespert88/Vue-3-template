<template>
  <div class="app">
    <AppNavbar />
    <router-view />
    <AppFooter />
  </div>
</template>
<script>
import AppNavbar from "./components/AppNavbar.vue";
import AppFooter from "./components/AppFooter.vue";
export default {
  name: "app",
  components: {
    AppNavbar,
    AppFooter,
  },
};
</script>
<style>
</style>
