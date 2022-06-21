<template>
  <div>
    <div class="footercontainer">
      <div class="container">
        <div class="d-flex justify-content-between align-items-center">
          <div class="d-flex flex-column">we</div>
          <div><img src="../assets/img/dc-logo-bg.png" alt="" srcset="" /></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheFooter",
};
</script>

<style lang="scss">
.footercontainer {
  height: 360px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;

  img {
   position: relative;
   transform: translateY(-20%);
    text-align: center;
  }
}
</style>
