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
    <a href="#">
      <div class="scroll-top">
        <i class="fas fa-arrow-up"></i>
    </div>
    </a>
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

#app {
  position: relative;
  .scroll-top {
    width: 50px;
    height: 50px;
    border-radius: 5px;
    background-color: $detailsColor;
    position: fixed;
    bottom: 30px;
    right: 30px;
    line-height: 50px;
    text-align: center;
    a {
      width: 50px;
      height: 50px;
      background-color: red;
    }
    .fa-arrow-up {
      color: $white;
      font-size: 1.6rem;
      padding-top: 12px;
    }
  }
}

</style>
