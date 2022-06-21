<template>
  <div>
      <TheNavbar />
      <BannerBlue />
      <TheFooter />
  </div>
</template>

<script>
import TheNavbar from "./components/TheNavbar.vue";
import BannerBlue from "./components/BannerBlue.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  name: "App",
  components: { TheNavbar, BannerBlue, TheFooter },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;700&display=swap");

* {
  font-family: "Asap Condensed", sans-serif;
}
</style>
