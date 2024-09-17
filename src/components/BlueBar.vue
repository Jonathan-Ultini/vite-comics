<template>
  <section class="blue-bar container-fluid py-3">
    <div class="row justify-content-center">
      <div class="col-6 col-md-2 text-center" v-for="icon in icons" :key="icon.title">
        <img :src="icon.image" :alt="icon.title" class="icon-image img-fluid mb-2" />
        <p class="text-white mb-0">{{ icon.title }}</p>
      </div>
    </div>
  </section>
</template>


<script>
export default {
  data() {
    return {
      icons: [
        { title: 'Digital Comics', image: '/src/assets/buy-comics-digital-comics.png' },
        { title: 'DC Merchandise', image: '/src/assets/buy-comics-merchandise.png' },
        { title: 'Subscription', image: '/src/assets/buy-comics-subscriptions.png' },
        { title: 'Comic Shop Locator', image: '/src/assets/buy-comics-shop-locator.png' },
        { title: 'DC Power Visa', image: '/src/assets/buy-dc-power-visa.svg' }
      ]
    };
  }
}
</script>

<style scoped lang="scss">
.blue-bar {
  position: relative;
  z-index: 3;
  background-color: #0282F9;

  .icon-image {
    max-width: 60px;
    max-height: 60px;
  }

  p {
    font-size: 14px;
  }
}
</style>
