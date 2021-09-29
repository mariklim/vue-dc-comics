<template>
  <div id="app">
    <Header/>
    <main> <Content/></main>
    <Footer/>

    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Content from './components/Content.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Content
  }
}
</script>

<style lang="scss">
@import "./assets/style/common";
</style>
