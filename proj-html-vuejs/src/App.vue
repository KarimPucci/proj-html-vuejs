<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppFooter,
  },
};
</script>

<template>
  <div class="container">
    <AppHeader />
    <AppJumbotron />
    <AppMain />
    <AppFooter />
  </div>
</template>

<style lang="scss">
</style>