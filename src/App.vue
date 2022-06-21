<template>
  <div>
    <div class="container">
      <TheNavbar />
    </div>
  </div>
</template>

<script>
import TheNavbar from "./components/TheNavbar.vue";

export default {
  name: "App",
  components: { TheNavbar },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Asap+Condensed:wght@400;700&display=swap");

* {
  font-family: "Asap Condensed", sans-serif;
}
</style>
