<template>
  <div id="app">
    <Header/>
    <Hero/>
    <SectionOne/>
    <SectionTwo/>
    <SectionThree/>
    <SectionFour/>
    <SectionFive/>
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

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive
  }
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";

// #app {
  
// }

</style>
