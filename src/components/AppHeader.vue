<script>
import AppMenu from "./AppMenu.vue";

export default {
  data() {
    return {
      items: [
        {
          title: "CHARACTERS",
          link: "#",
        },
        {
          title: "COMICS",
          link: "#",
        },
        {
          title: "MOVIES",
          link: "#",
        },
        {
          title: "TV",
          link: "#",
        },
        {
          title: "GAMES",
          link: "#",
        },
        {
          title: "COLLECTIBLES",
          link: "#",
        },
        {
          title: "VIDEOS",
          link: "#",
        },
        {
          title: "FANS",
          link: "#",
        },
        {
          title: "NEWS",
          link: "#",
        },
        {
          title: "SHOP",
          link: "#",
        },
      ],
    };
  },
  components: { AppMenu },
};
</script>

<template>
  <header>
    <div class="bg_header">
      <img src="../assets/img/dc-logo.png" alt="logo-DC" />
      <AppMenu :menuItems="items" />
    </div>
    <div class="jumbotron">
      <button><a href="#">CURRENT SERIES</a></button>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "./../assets/style/partials/variables.scss" as *;

header {
  background-color: white;
  color: black;
}

.bg_header {
  margin: auto;
  max-width: 1200px;
  display: flex;
  justify-content: space-between;
}

header img {
  padding: 0.5rem;
  cursor: pointer;
}

.jumbotron {
  background-image: url(../assets/img/jumbotron.jpg);
  height: 25rem;
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
  button {
    background-color: #0282f9;
    padding: 0.7rem;
    position: absolute;
    bottom: -22px;
    left: 21rem;
    &:hover {
      background-color: #0e68bd;
    }
    a {
      font-size: 1.3em;
      color: white;
      text-decoration: none;
    }
  }
}
</style>
