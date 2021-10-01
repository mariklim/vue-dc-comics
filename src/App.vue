<template>
  <div id="app">
    <Header/>
    <main> 
     <Hero :src="require('./assets/img/jumbotron.jpg')" />
    <Content/>
    </main>
    <Footer/>

    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Content from './components/Content.vue'
import Hero from './components/Hero.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Content,
    Hero,
  }
}
</script>

<style lang="scss">
@import "./assets/style/common";
</style>
