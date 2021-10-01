<template>
  <div id="app">
    <Header/>
    <main>
      <SectionHero :src="require('./assets/img/jumbotron.jpg')" />
      <SectionSeries/>
      <SectionBuy/>
    </main>
    <Footer/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue';
import SectionHero from './components/SectionHero.vue';
import SectionSeries from './components/SectionSeries.vue';
import SectionBuy from './components/SectionBuy.vue';
import Footer from './components/Footer.vue';



export default {
  name: 'App',
  components: {
    // HelloWorld
    Header,
    SectionHero,
    SectionSeries,
    SectionBuy,
    Footer
  }
}
</script>

<style lang="scss">
  @import 'assets/scss/common.scss';
</style>
