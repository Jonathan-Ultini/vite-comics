<template>
  <div>
    <Header />
    <MainContent />
    <BlueBar />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import BlueBar from './components/BlueBar.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    MainContent,
    BlueBar,
    Footer
  }
}
</script>

<style lang="scss">
@import 'bootstrap/dist/css/bootstrap.min.css';
</style>
