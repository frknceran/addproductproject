<template>
  <div id="app">
  <appNavbar></appNavbar>
 <div :style="bgImg">
 <app-campain></app-campain>
 <app-card></app-card>
 <app-carousel></app-carousel>
 <app-ramazan-ozel></app-ramazan-ozel>
 </div>
 <app-footer></app-footer>
  </div>
</template>

<script>
import appNavbar from "./components/Navbar.vue";
import appCampain from "./components/Campain.vue";
import appCard from "./components/Card.vue";
import appCarousel from "./components/Carousel.vue";
import appRamazanOzel from "./components/RamazanOzel.vue";
import appFooter from "./components/Footer.vue";

export default {
  name: 'App',
  components: {
    appNavbar,
    appCampain,
    appCard,
    appCarousel,
    appRamazanOzel,
    appFooter

  },
    data() {
      return {
        bgImg: {
          backgroundImage: `url(${require('./assets/backgorunddd.jpg')})`
        }
      }
    }
  }

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 10px;
}
</style>
