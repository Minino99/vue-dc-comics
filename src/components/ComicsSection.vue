<template>
  <div>
        <TheJumbotron :jumbo-img="ClickedComic"/>
    <div class="comicssection">
      <div class="container h-100 p-4 py-5">
        <div class="row h-100">
          <div class="col lg-2" v-for="comic in Comics" :key="comic.series">
            <div class="squareimg mb-3">
              <a href="#" @click="ClickComic(comic)">
              <img :src="comic.thumb" :alt="comic.series" srcset=""
              /></a>
            </div>
            <div class="comicname">{{ comic.series.toUpperCase() }}</div>
          </div>
        </div>
        <div class="mt-4 mb-0 text-center">
            <button type="button" class="btn mybtn btn-lg px-5">
              LOAD MORE
            </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TheJumbotron from "./TheJumbotron.vue";
export default {
  name: "ComicsSection",
  components: { TheJumbotron },
  data: function () {
    return {
      ClickedComic: "https://images4.alphacoders.com/646/thumb-1920-646026.jpg",
      Comics: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
          bg: "https://images.wallpapersden.com/image/download/superman-action-comics-dc-comics_ZmVpa26UmZqaraWkpJRmbmdlrWZlbWU.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
          bg: "https://images.hdqwalls.com/download/american-vampire-1976-sz-1920x1080.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
          bg: "https://images7.alphacoders.com/973/973272.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
          bg: "https://images4.alphacoders.com/164/thumb-1920-164246.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
          bg: "https://wallpaperaccess.com/full/525044.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
          bg: "https://images.alphacoders.com/807/thumb-1920-807852.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
          bg:"https://images3.alphacoders.com/103/thumb-1920-1033030.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
          bg:"https://p4.wallpaperbetter.com/wallpaper/996/740/36/batman-and-superman-batman-and-superman-wallpaper-preview.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
          bg: "https://www.dccomics.com/sites/default/files/Gallery_20200930_Batman_JokerWarZone_Variant_5f627728d05877.02872275.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
          bg: "https://i0.wp.com/www.comicsuniverse.it/wp-content/uploads/2020/08/3-joker-1920x1080-1.jpg?ssl=1",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
          bg: "https://images5.alphacoders.com/872/872431.jpg",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
          bg: "https://images.alphacoders.com/871/871607.jpg",
        },
      ],
    };
  },
  methods: {
    ClickComic(comic) {
      this.ClickedComic = comic.bg;
    },
  },
};
</script>

<style lang="scss" scoped>
.comicssection {
  background-color: #101010;
  min-height: 620px;
}
.squareimg {
  width: 192px;
  height: 192px;
  overflow: hidden;
}
.comicname {
  color: white;
  height: 48px;
}

.mybtn{
  color: white;
  font-size: 1rem;
  font-weight: 700;
  border-radius: 0;
  background-color: #0081EF;
}
</style>
