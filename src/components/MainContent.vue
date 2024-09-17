<template>
  <div class="main-content-wrapper bg-dark">
    <main class="main-content container py-5">
      <h2 class="text-white mb-4 btn btn-primary">Current Series</h2>
      <div class="row">
        <Card v-for="(comic, index) in comics" :key="index" :thumb="comic.thumb" :series="comic.series"
          :price="comic.price" :type="comic.type" />
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

<style scoped lang="scss"></style>
