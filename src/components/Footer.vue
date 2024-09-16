<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-section">
        <h3>DC Comics</h3>
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Collectibles</a></li>
        </ul>
      </div>

      <div class="footer-section">
        <h3>DC</h3>
        <ul>
          <li><a href="#">DC Merchandise</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Comic Shop Locator</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>

      <div class="footer-section">
        <h3>Follow Us</h3>
        <div class="social-links">
          <a href="#"><img src="/src/assets/footer-facebook.png" alt="Facebook"></a>
          <a href="#"><img src="/src/assets/footer-twitter.png" alt="Twitter"></a>
          <a href="#"><img src="" alt="YouTube"></a>
          <a href="#"><img src="/src/assets/footer-pinterest.png" alt="Pinterest"></a>
          <a href="#"><img src="/src/assets/footer-periscope.png" alt="Location"></a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
.footer {
  background-color: #000;
  color: white;
  padding: 20px 0;
}

.footer-content {
  display: flex;
  justify-content: space-around;
}

.footer-section h3 {
  margin-bottom: 10px;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section ul li {
  margin-bottom: 5px;
}

.footer-section ul li a {
  color: white;
  text-decoration: none;
}

.footer-section ul li a:hover {
  text-decoration: underline;
}

.social-links a img {
  width: 24px;
  margin-right: 10px;
}
</style>
