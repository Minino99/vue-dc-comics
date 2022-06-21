<template>
  <div>
    <div class="container">
      <nav
        class="navbar navbar-light justify-content-between align-items-center"
        style="padding-bottom: 0px; padding-top: 0px"
      >
        <div class="navbar-brand py-2">
          <a><img src="../assets/img/dc-logo.png" alt="DC Logo" srcset="" /></a>
        </div>
        <div class="d-flex gap-4 navelements">
          <div
            class="dcnavelement"
            v-for="navelement in navElements"
            :key="navelement.name"
          >
            <a :href="navelement.link">{{ navelement.name }}</a>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheNavbar",
  data() {
    return {
      navElements: [
        {
          name: "CHARACTERS",
          link: "#",
        },
        {
          name: "COMICS",
          link: "#",
        },
        {
          name: "MOVIES",
          link: "#",
        },
        {
          name: "TV",
          link: "#",
        },
        {
          name: "GAMES",
          link: "#",
        },
        {
          name: "COLLECTIBLES",
          link: "#",
        },
        {
          name: "VIDEOS",
          link: "#",
        },
        {
          name: "FANS",
          link: "#",
        },
        {
          name: "NEWS",
          link: "#",
        },
        {
          name: "SHOP",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.navbar {
  height: 100px;

  .navbar-brand {
    height: 100%;
  }
  img {
    height: 100%;
  }
}

.navelements {
  height: 100%;

  .dcnavelement {
    height: 100%;
    display: flex;
    align-items: center;
    border-bottom: solid 5px transparent;
    font-size: 0.9rem;

    &:hover {
      border-bottom: solid 5px #0081ef;
    }

    &:hover a {
      color: #0081ef;
    }

    a {
      color: black;
      text-decoration: none;
    }
  }
}
</style>
