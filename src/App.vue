<template>
  <div id="app">
    <Header />
    <main>
      <Hero :src="require('./assets/img/jumbotron.jpg')" />
      <MainTop />
      <MainBottom />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import MainBottom from "./components/MainBottom.vue";
import Hero from "./components/Hero.vue";
import MainTop from "./components/MainTop.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
    MainBottom,
    Hero,
    MainTop,
  },
};
</script>

<style lang="scss">
@import "./assets/style/common";
</style>
