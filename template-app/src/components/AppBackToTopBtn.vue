<template>
  <div>
    <BackToTop bottom="30px" right="30px">
      <button type="button" class="btn-to-top">
        <i class="fa fa-chevron-up"></i>
      </button>
    </BackToTop>
  </div>
</template>

<script>
import BackToTop from "vue-backtotop";
export default {
  components: { BackToTop },
};
</script>

<style>
@import "../assets/css/globalStyles.css";
/* in your css */
.btn-to-top {
  width: 40px;
  height: 40px;
  padding: 4px;
  border-radius: 50%;
  font-size: 22px;
  line-height: 22px;

  border: 0;
  color: var(--white);
  background-color: var(--lightBlue);
}
</style>