<script>
export default {
  name: "AppFooter"

};
</script>

<template>
  <footer>
    <div class="footer-top">
      <div class="container flex">
        <!-- Footer-Left -->
        <div id="dc-comics">
          <h4>DC COMICS</h4>
          <ul>
            <li>
              <a href="#">Characters</a>
            </li>
            <li>
              <a href="#">Comics</a>
            </li>
            <li>
              <a href="#">Movies</a>
            </li>
            <li>
              <a href="#">TV</a>
            </li>
            <li>
              <a href="#">Games</a>
            </li>
            <li>
              <a href="#">Videos</a>
            </li>
            <li>
              <a href="#">News</a>
            </li>
          </ul>
          <!-- ------------------ -->
          <h4>SHOP</h4>
          <ul>
            <li>
              <a href="#">Shop DC</a>
            </li>
            <li>
              <a href="#">Shop DC Collectibles</a>
            </li>
          </ul>
        </div>
        <!-- Footer-Mid -->
        <div id="dc">
          <h4>DC</h4>
          <ul>
            <li>
              <a href="#">Term Of Use</a>
            </li>
            <li>
              <a href="#">Privacy policy(New)</a>
            </li>
            <li>
              <a href="#">Ad Choises</a>
            </li>
            <li>
              <a href="#">Advertising</a>
            </li>
            <li>
              <a href="#">Jobs</a>
            </li>
            <li>
              <a href="#">Subscriptions</a>
            </li>
            <li>
              <a href="#">Talent Workshops</a>
            </li>
            <li>
              <a href="#">CPSC Certificates</a>
            </li>
            <li>
              <a href="#">Rating</a>
            </li>
            <li>
              <a href="#">Shop Help</a>
            </li>
            <li>
              <a href="#">Contact Us</a>
            </li>
          </ul>
        </div>
        <!-- Footer-Right -->
        <div id="sites">
          <h4>SITES</h4>
          <ul>
            <li>
              <a href="#">DC</a>
            </li>
            <li>
              <a href="#">Mad Magazine</a>
            </li>
            <li>
              <a href="#">DC Kids</a>
            </li>
            <li>
              <a href="#">DC Universe</a>
            </li>
            <li>
              <a href="#">DC Power Visa</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <!-- Footer-Bottom -->
    <div class="footer-bottom">
      <div class="container flex2">
        <div>
          <button>SIGN-UP NOW!</button>
        </div>
        <div class="flex2">
          <p>FOLLOW US</p>
          <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
          <a href="#"><img src="../assets/img/footer-twitter.png" alt="X"></a>
          <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
          <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
          <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.container {
  max-width: 1200px;
  margin: 0 auto;
}

.flex {
  display: flex;
  gap: 20px;
}

.flex2 {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
  gap: 20px;
}

footer {
  color: white;
  max-height: 400px;
}

footer li {
  margin: 6px 0;
  font-size: 0.8rem;
}

.footer-top {

  gap: 20px;
  background-image: url(../assets/img/footer-bg.jpg);
  height: 400px;

}

ul {
  list-style: none;
  padding: 0;
}

a {
  text-decoration: none;
  color: grey;
  text-align: start;
}

.footer-bottom {
  height: 80px;
  background-color: #303030;
}

button {
  color: white;
  background-color: #303030;
  padding: 15px;
  border: 2px solid #0282F9;

}
</style>
