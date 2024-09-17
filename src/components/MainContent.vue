<template>
  <div class="hero-image"></div>
  <div class="main-content-wrapper bg-dark">
    <main class="main-content container py-5">
      <h2 class="text-white mb-4 btn btn-primary">Current Series</h2>
      <div class="row">
        <Card v-for="(comic, index) in comics" :key="index" :thumb="comic.thumb" :series="comic.series"
          :price="comic.price" :type="comic.type" />
      </div>
      <div class="text-center mt-4">
        <button class="btn btn-primary">Load More</button>
      </div>
    </main>
  </div>
</template>


<script>
import Card from './Card.vue';
import comicsData from '../assets/comics.json';

export default {
  name: 'MainContent',
  components: {
    Card,
  },
  data() {
    return {
      comics: comicsData,
    };
  },
};
</script>

<style scoped lang="scss">
.hero-image {
  background-image: url('./src/assets/jumbotron.jpg');
  background-size: cover;
  background-position: center top;
  background-repeat: no-repeat;
  height: 300px;
  width: 100%;
}
</style>
