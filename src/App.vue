<template>
  <div id="app">
    <Header/>
    <Hero/>
    <SectionOne/>
    
    
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import SectionOne from './components/SectionOne.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    SectionOne
  }
}
</script>

<style lang="scss">
@import "./assets/style/common.scss";

// #app {
  
// }

</style>
