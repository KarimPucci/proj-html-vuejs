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
  <div class="container d-flex">
    <img :src="getPathImage(immagine)" alt="logo" />

    <nav>
      <a href="#">HOMES</a>
      <a href="#">PAGES</a>
      <a href="#">BLOG</a>
      <a href="#">SHOP</a>
      <a href="#">EVENTS</a>
      <a href="#">ELEMENTS</a>
    </nav>
  </div>
</template>

<style scoped>
</style>