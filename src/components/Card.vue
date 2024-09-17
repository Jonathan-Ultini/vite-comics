<!-- components/Card.vue -->
<template>
  <div class="card">
    <img :src="thumb" :alt="series" />
    <div class="card-body">
      <h5 class="card-title">{{ series }}</h5>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    thumb: String,
    series: String
  },
};
</script>

<style scoped lang="scss">
.card {
  width: 200px;
  margin: 10px;

  img {
    width: 100%;
    height: auto;
  }

  .card-body {
    background-color: #333;
    color: white;
    text-align: center;
  }
}
</style>
