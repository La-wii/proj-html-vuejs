<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <Courses/>
    <Program/>
    <Youtube/>
    <Slide/>
    <Cta/>
    <Count/>
    <Blog/>
    <Newsletters/>
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
import Program from './components/Program.vue';
import Youtube from './components/Youtube.vue';
import Slide from './components/Slide.vue';
import Cta from './components/Cta.vue';
import Count from './components/Count.vue';
import Blog from './components/Blog.vue';
import Newsletters from './components/Newsletters.vue';
import Footer from './components/Footer.vue';
export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    Courses,
    Program,
    Youtube,
    Slide,
    Cta,
    Count,
    Blog,
    Newsletters,
    Footer,
  },
};
</script>

<style lang="scss">
@import '@/style/common.scss';

</style>
