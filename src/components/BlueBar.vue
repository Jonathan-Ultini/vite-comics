<template>
  <section class="blue-bar">
    <div class="icon-section" v-for="icon in icons" :key="icon.title">
      <img :src="icon.image" :alt="icon.title" class="icon-image" />
      <p>{{ icon.title }}</p>
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
  background-color: #0282F9;
  display: flex;
  justify-content: space-around;
  padding: 15px 0;

  .icon-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: white;

    .icon-image {
      width: 50px;
      height: 50px;
      margin-bottom: 5px;
    }

    p {
      font-size: 12px;
      text-align: center;
      margin: 0;
    }
  }
}
</style>
