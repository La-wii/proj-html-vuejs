<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "@/components/Header.vue";  
import Jumbotron from './components/Jumbotron.vue';
export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
  },
};
</script>

<style lang="scss">
@import '@/style/common.scss';

</style>
