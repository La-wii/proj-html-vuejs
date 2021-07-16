<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <Courses/>
    <Footer/>
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "@/components/Header.vue";  
import Jumbotron from './components/Jumbotron.vue';
import Courses from './components/Courses.vue';
import Footer from './components/Footer.vue';
export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    Courses,
    Footer,
  },
};
</script>

<style lang="scss">
@import '@/style/common.scss';

</style>
