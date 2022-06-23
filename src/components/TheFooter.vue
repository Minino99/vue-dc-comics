<template>
  <div>
    <div class="footercontainer">
      <div class="container">
        <div class="d-flex justify-content-between h-100">
          <div class="d-flex flex-column flex-wrap gap-3 py-5 footerlinks">
            <div
              class="footerelement"
              v-for="elemento in footerElements"
              :key="elemento.title"
            >
              <div class="title pb-2">{{ elemento.title }}</div>
              <div class="text" v-for="(link, i) in elemento.links" :key="i">
                {{ link }}
              </div>
            </div>
          </div>
          <div class="of-hidden">
            <img src="../assets/img/dc-logo-bg.png" alt="" srcset="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheFooter",
  data: function () {
    return {
      footerElements: [
        {
          title: "DC COMICS",
          links: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },
        {
          title: "SHOP",
          links: ["Shop DC", "Shop DC Collectibles"],
        },
        {
          title: "DC",
          links: [
            "Terms Of Use",
            "Privacy Policy (New)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshps",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },
        {
          title: "SITES",
          links: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.text {
  color: #494949;
  font-size: 0.8rem;
}

.title {
  color: white;
  font-size: 1.2rem;
}

.footercontainer {
  height: 360px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;

  .container {
    height: 100%;
  }

  img {
    position: relative;
    transform: translateY(-20%);
    text-align: center;
  }

  .of-hidden {
    max-height: 100%;
    overflow: hidden;
  }
}
</style>
