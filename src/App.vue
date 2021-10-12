<template>
  <div id="app">
    <Header/>
    <Hero/>
    <SectionOne/>
    <SectionTwo/>
    <SectionThree/>
    <SectionFour/>
    <SectionFive/>
    <SectionSix/>
    <SectionSeven/>
    <SectionEight/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import SectionOne from './components/SectionOne.vue';
import SectionTwo from './components/SectionTwo.vue';
import SectionThree from './components/SectionThree.vue';
import SectionFour from './components/SectionFour.vue';
import SectionFive from './components/SectionFive.vue';
import SectionSix from './components/SectionSix.vue';
import SectionSeven from './components/SectionSeven.vue';
import SectionEight from './components/SectionEight.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Hero,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    SectionSeven,
    SectionEight,
    Footer
  }
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";

// #app {
  
// }

</style>
