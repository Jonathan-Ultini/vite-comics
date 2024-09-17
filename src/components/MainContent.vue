<template>
  <main class="main-content container">
    <h2>Current Series</h2>
    <div class="row">
      <Card v-for="(comic, index) in comics" :key="index" :thumb="comic.thumb" :series="comic.series"
        :price="comic.price" :type="comic.type" />
    </div>
  </main>
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
.main-content {
  background-color: #1C1C1C;
  padding: 20px;

  h2 {
    color: #fff;
    font-weight: bold;
    margin-bottom: 20px;
  }

  .row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>
