<template>
  <footer>
      <div class="upper-footer">
          <div class="container"> 
            <div class="links-list">
                <div class="col">
                    <ul>
                        <li class="list-title">DC comics</li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">Tv</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <ul>
                        <li class="list-title">Shop</li>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <li class="list-title">DC</li>
                        <li><a href="#">Terms of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choises</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscription</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="col">
                    <ul>
                        <li class="list-title">Sites</li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
          </div>
      </div>
      <div class="down-footer">
          <div class="container footer">
              <div class="sign-up">
                  <a href="#">Sign up</a>
                </div>
                <div class="social-icons">
                    <h3>FOLLOW US</h3>
                    <a href="#"><img src="..\assets\img\footer-facebook.png" alt="facebook"></a>
                    <a href="#"><img src="..\assets\img\footer-periscope.png" alt="periscope"></a>
                    <a href="#"><img src="..\assets\img\footer-pinterest.png" alt="pinterest"></a>
                    <a href="#"><img src="..\assets\img\footer-twitter.png" alt="twitter"></a>
                    <a href="#"><img src="..\assets\img\footer-youtube.png" alt="youtube"></a>
                </div>
          </div>
      </div>

  </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped>

ul {
    margin-bottom: 20px;
}

ul li {
    margin-bottom: 5px;
}

ul li a {
    color: gray;
    font-weight: normal;
}

.upper-footer {
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
}

.links-list {
    display: flex;
    padding: 20px 0;
}

.col {
    margin-right: 30px;
    color: white;
}

.list-title {
    font-size: 20px;
    font-weight: bold;
    margin-bottom: 10px;
    text-transform: uppercase;
}

.down-footer {
    height: 110px;
    background-color: #303030;
}

.container.footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.sign-up a {
   text-transform: uppercase;
    padding: 10px 25px;
    border: 2px solid dodgerblue;
    color: white;
    font-size: 20px;
}

.social-icons {
    display: flex;
    align-items: center;
}

.social-icons a{
    margin-left: 15px;
}

.social-icons h3 {
    color: dodgerblue;
}

</style>