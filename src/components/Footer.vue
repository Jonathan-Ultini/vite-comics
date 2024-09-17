<template>
  <footer class="footer">
    <div class="footer-background">
    </div>
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
          <li><a href="#">Term Of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choces</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscription</a></li>
          <li><a href="#">Talent Workdhops</a></li>
          <li><a href="#">CPSC Certificaates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>

      <div class="footer-section">
        <h3>Sites</h3>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">Mad Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
        </ul>
      </div>

    </div>

    <div class="footer-bottom">
      <button class="signup-button">SIGN-UP NOW!</button>
      <div class="social-media">
        <p class="blue">FOLLOW US</p>
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

<style scoped lang="scss">
.footer {
  background-color: #2c2c2c;
  color: white;

  .footer-background {
    position: absolute;
    top: 300px;
    left: 100px;
    right: -500px;
    height: 50%;
    z-index: 1;
    background-image: url("/src/assets/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
  }

  .footer-content {
    display: flex;
    background-image: url("/src/assets/footer-bg.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    min-height: 300px;
  }

  .footer-section {
    margin: 0 20px;

    h3 {
      color: #fff;
      font-weight: bold;
      text-transform: uppercase;
      margin-bottom: 15px;
    }

    ul {
      list-style: none;
      padding: 0;

      li a {
        color: grey;
        text-decoration: none;
        font-size: 14px;

        &:hover {
          text-decoration: underline;
        }
      }
    }
  }

  .footer-bottom {
    display: flex;
    justify-content: space-between;
    padding: 20px;
    background-color: #303030;

    .signup-button {
      background-color: transparent;
      color: white;
      padding: 10px 20px;
      border: 2px solid #0282F9;

      &:hover {
        background-color: #008bc5;
      }
    }

    .blue {
      color: #0282F9;
      font-weight: bold;
    }

    .social-media {
      color: white;

      .social-links a img {
        width: 24px;
        margin-right: 10px;
      }
    }
  }
}
</style>
