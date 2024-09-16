<template>
  <nav class="header">
    <img src="/src/assets/dc-logo.png" alt="DC Logo" class="logo">
    <ul class="menu">
      <li v-for="item in menuItems" :key="item">
        <a href="#" class="menu-link">{{ item }}</a>
      </li>
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
  background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
  border-bottom: 2px solid #ccc;
}

.logo {
  width: 100px;
}

.menu {
  list-style: none;
  display: flex;
  gap: 15px;
  margin: 0;
  padding: 0;
}

.menu-link {
  color: black;
  text-decoration: none;
  font-size: 14px;
  text-transform: uppercase;
}

.menu-link:hover {
  border-bottom: 2px solid blue;
}
</style>
