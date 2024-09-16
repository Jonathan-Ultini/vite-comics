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
        <h3>Shop</h3>
        <ul>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
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
        <h3>Sites</h3>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">Mad Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>




    </div>

    <div class="footer-bottom">
      <button class="signup-button">SIGN-UP NOW!</button>
      <div class="social-media">
        <p>FOLLOW US</p>
        <div class="social-links">
          <a href="#"><img src="/src/assets/footer-facebook.png" alt="Facebook"></a>
          <a href="#"><img src="/src/assets/footer-twitter.png" alt="Twitter"></a>
          <a href="#"><img src="/src/assets/footer-youtube.png" alt="YouTube"></a>
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
  background-color: #2c2c2c;
  color: white;
}

.footer-content {
  display: flex;
  justify-content: space-around;
  background-image: url("/src/assets/footer-bg.jpg");
  background-size: auto;
  background-position: center;
  min-height: 300px;
}


.footer-section h3 {
  color: #00AEEF;
  margin-bottom: 15px;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section ul li a {
  color: white;
  text-decoration: none;
  font-size: 14px;
}

.footer-section ul li a:hover {
  text-decoration: underline;
}

.social-links a img {
  width: 24px;
  margin-right: 10px;
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background-color: #303030;
}

.signup-button {
  background-color: #00AEEF;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}

.signup-button:hover {
  background-color: #008bc5;
}

.social-media {
  color: white;
}

.social-media p {
  margin: 0;
}
</style>
