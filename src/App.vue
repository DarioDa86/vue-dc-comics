<template>
  <div id="app">
    <Header/>
    <MainTop>

    </MainTop>
    <MainBottom>

    </MainBottom>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainTop from './components/MainTop.vue';
import MainBottom from './components/MainBottom.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    MainBottom,
    Footer
  }
}
</script>

<style lang="scss">
  @import '../src/assets/style/common';
  @import '../src/assets/style/variables';
</style>
