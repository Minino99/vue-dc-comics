<template>
  <div>
    <div class="bannerblue">
      <div class="container h-100">
        <div class="row justify-content-center align-items-center h-100">
          <div
            class="col d-flex align-items-center gap-3"
            v-for="bluebannerelement in buyElements"
            :key="bluebannerelement.text"
          >
              <img :src="bluebannerelement.img" alt="" srcset="" class="icon" />
              <span>{{ bluebannerelement.text }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerBlue",
  data: function () {
    return {
      buyElements: [
        {
          text: "DIGITAL COMICS",
          img: "img/buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          img: "img/buy-comics-merchandise.png",
        },
        {
          text: "SUBSCRIPTION",
          img: "img/buy-comics-subscriptions.png",
        },
        {
          text: "COMIC SHOP LOCATOR",
          img: "img/buy-comics-shop-locator.png",
        },
        {
          text: "DC POWER VISA",
          img: "img/buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.bannerblue {
  background-color: #0081ef;
  color: white;
  height: 180px;
}

.icon {
  max-height: 50px;
  max-width: 50px;
}


</style>
