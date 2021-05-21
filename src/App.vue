<template>
  <div id="app">
    <Header />
    <Main />
    <Commercial />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header'
import Main from './components/Main'
import Commercial from './components/Commercial'
import Footer from './components/Footer'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Commercial,
    Footer
    
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
@import './assets/style/utilities.scss';



</style>
