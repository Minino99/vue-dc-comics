<template>
  <div>
    <TheNavbar />
    <TheJumbotron />
    <ComicsSection :jumbo-img="ClickedComic" />
    <BannerBlue />
    <TheFooter />
    <BannerSignUp />
  </div>
</template>

<script>
import TheNavbar from "./components/TheNavbar.vue";
import TheJumbotron from "./components/TheJumbotron.vue";
import ComicsSection from "./components/ComicsSection.vue";
import BannerBlue from "./components/BannerBlue.vue";
import TheFooter from "./components/TheFooter.vue";
import BannerSignUp from "./components/BannerSignUp.vue";

export default {
  name: "App",
  components: { TheNavbar, TheJumbotron, ComicsSection, BannerBlue, TheFooter, BannerSignUp, },
  
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;700&display=swap");

* {
  font-family: "Asap Condensed", sans-serif !important;
}
</style>
