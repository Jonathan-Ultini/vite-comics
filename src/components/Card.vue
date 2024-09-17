<template>
  <div class="col-lg-2 col-md-4 col-sm-4 mb-4">
    <div class="card h-100">
      <img :src="thumb" :alt="series" class="card-img-top" />
      <div class="card-body text-center">
        <h5 class="card-title text-white">{{ series }}</h5>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  props: {
    thumb: String,
    series: String,
  }
};
</script>

<style scoped lang="scss">
.card {
  background-color: #333;
  border: none;

  .card-img-top {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }

  .card-body {
    background-color: #1C1C1C;
  }

  h5 {
    font-size: 1.1rem;
  }
}
</style>
