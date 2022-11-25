<script>
export default {
  name: "AppHeader",
  data() {
    return {
      immagine: "logo-img-01.png",
    };
  },
  methods: {
    getPathImage(imageName) {
      return new URL(`../teach/img/${imageName}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="container d-flex justify-content-space-between">
    <img :src="getPathImage(immagine)" alt="logo" />

    <nav>
      <ul class="menu d-flex">
        <li>
          <i class="fa-thin fa-arrow-right"></i>
          <a href="#">HOMES</a>
        </li>
        <li>
          <a href="#">PAGES</a>
        </li>
        <li>
          <a href="#">BLOG</a>
        </li>
        <li>
          <a href="#">SHOP</a>
        </li>
        <li>
          <a href="#">EVENTS</a>
        </li>
        <li>
          <a href="#">ELEMENTS</a>
        </li>
        <li>
          <i class="fa-light fa-magnifying-glass"></i>
        </li>
        <li>
          <i class="fa-regular fa-bars"></i>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 30px;
  margin-top: 10px;
}

.menu {
  margin-left: 600px;
}

a {
  padding: 10px;
  text-decoration: none;
  color: black;
}

li {
  list-style: none;
}
</style>