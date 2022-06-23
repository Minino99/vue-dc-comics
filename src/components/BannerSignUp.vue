<template>
  <div>
    <div class="bannersignupcontainer">
      <div class="container h-100">
        <div class="row align-items-center justify-content-between h-100">
          <div class="col">
            <button type="button" class="btn btn-outline-primary signupbtn">
              SIGN-UP NOW!
            </button>
          </div>
          <div class="col socialslink d-flex justify-content-end gap-4 align-items-center">
            <span>FOLLOW US</span>
            <img v-for="logo in socialLogos" :key="logo.name" :src="logo.icon" :alt="logo.name">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerSignUp",
  data: function () {
    return {
      socialLogos: [
        {
          name: "facebook",
          icon: "img/footer-facebook.png",
        },
        {
          name: "twitter",
          icon: "img/footer-twitter.png",
        },
        {
          name: "youtube",
          icon: "img/footer-youtube.png",
        },
        {
          name: "pinterest",
          icon: "img/footer-pinterest.png",
        },
        {
          name: "periscope",
          icon: "img/footer-periscope.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.bannersignupcontainer {
  background-color: #282828;
  height: 100px;
}

.signupbtn {
  border-radius: 0 !important;
  border: 2px solid #0081ef !important;
  color: white !important;
  font-size: 1.2rem !important;
}

.socialslink span{
  color: #0081ef;
  font-weight: 700;
  font-size: 1.5rem;
}
</style>
