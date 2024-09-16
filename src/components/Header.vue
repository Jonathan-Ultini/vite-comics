<template>
  <nav class="header">
    <img src="/src/assets/dc-logo.png" alt="DC Logo" class="logo">
    <ul class="menu">
      <li v-for="item in menuItems" :key="item">{{ item }}</li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      menuItems: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Collectibles', 'Videos', 'Fans', 'News', 'Shop']
    };
  }
}
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  background-color: #fff;
}

.logo {
  width: 50px;
}

.menu {
  list-style: none;
  display: flex;
  gap: 20px;
}

.menu li {
  cursor: pointer;
}

.menu li:hover {
  color: blue;
}
</style>
