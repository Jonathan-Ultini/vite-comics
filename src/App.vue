<template>
  <div>
    <Header />
    <MainContent />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'

export default {
  components: {
    Header,
    MainContent
  }
}
</script>

<style>
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
</style>
