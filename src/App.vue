<template>
  <div id="app">
  <appNavbar></appNavbar>
 <div :style="bgImg">
 <app-campain></app-campain>
 <app-card></app-card>
 </div>
  </div>
</template>

<script>
import appNavbar from "./components/Navbar.vue";
import appCampain from "./components/Campain.vue";
import appCard from "./components/Card.vue"

export default {
  name: 'App',
  components: {
    appNavbar,
    appCampain,
    appCard

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
