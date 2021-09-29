<template>
  <div id="app">
    <Header/>
    <main>
      <SectionMistery/>
      <SectionBuy/>
    </main>
    <Footer/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import SectionMistery from './components/SectionMistery.vue'
import SectionBuy from './components/SectionBuy.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld
    Header,
    SectionMistery,
    SectionBuy,
    Footer
  }
}
</script>

<style lang="scss">
  @import 'assets/scss/common.scss';
</style>
