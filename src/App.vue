<template>
  <div>
    <Header />
    <MainContent />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    MainContent,
    Footer
  }
}
</script>

<style>
/* Stili globali */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

div {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

main {
  flex: 1;
}
</style>
