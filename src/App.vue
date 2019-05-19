<template lang="pug">
  #app
    <Header />
    <info />
    <Checkboxes />
    <LevelJS />
    <About />
    <Future />
    <Footer />
</template>

<script>
import Header from "./components/Header.vue";
import Info from "./components/Info.vue";
import Checkboxes from "./components/Checkboxes.vue";
import LevelJS from "./components/LevelJS.vue";
import About from "./components/About.vue";
import Future from "./components/Future.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "app",
  components: {
    Header,
    Info,
    Checkboxes,
    LevelJS,
    About,
    Future,
    Footer
  }
};
</script>

<style lang="stylus">

@font-face
  font-family: 'CourierNewPSMT'
  src: url("./assets/fonts/CourierNewPSMT.eot")
  src: url("./assets/fonts/CourierNewPSMT.eot?#iefix") format("embedded-opentype"),
       url("./assets/fonts/CourierNewPSMT.svg#CourierNewPSMT") format("svg"),
       url("./assets/fonts/CourierNewPSMT.ttf") format("truetype"),
       url("./assets/fonts/CourierNewPSMT.woff") format("woff"),
       url("./assets/fonts/CourierNewPSMT.woff2") format("woff2")
  font-weight: normal
  font-style: normal

@import url("https://fonts.googleapis.com/css?family=PT+Sans:400,700")

*
  padding: 0
  margin: 0
  box-sizing: border-box

#app
  font-family: "PT Sans", sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  font-size: 100%
  width: 100%
  max-width: 1000px
  background-image: url(./assets/images/BG-part.jpg)
  margin: 0 auto
  padding: 60px 115px

a
  color: #1f5f97

@media screen and (max-width: 960px)
  #app
    padding: 60px 40px

@media screen and (max-width: 767px)
  #app
    padding: 60px 10px
</style>
