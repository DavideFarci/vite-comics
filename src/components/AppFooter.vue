<script></script>

<template>
  <footer>
    <div class="nav_footer">
      <div class="container">
        <ul class="blu_nav">
          <li>
            <img
              src="../assets/img/buy-comics-digital-comics.png"
              alt="#"
            />DIGITAL COMICS
          </li>
          <li>
            <img src="../assets/img/buy-comics-merchandise.png" alt="#" />DC
            MERCHANDISE
          </li>
          <li>
            <img
              src="../assets/img/buy-comics-subscriptions.png"
              alt="#"
            />SUBSCRIPTION
          </li>
          <li>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="#" />COMIC
            SHOP LOCATOR
          </li>
          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="#" />DC POWER
            VISA
          </li>
        </ul>
      </div>
    </div>

    <div class="main_footer">
      <div class="container-f">
        <ul class="first_colums">
          <li>DC COMICS</li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>

          <li>SHOP</li>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>

        <ul>
          <li>DC</li>
          <li><a href="#">Terms of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>

        <ul>
          <li>SITES</li>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>

        <img src="../assets/img/dc-logo-bg.png" alt="logo-bg" />
      </div>
    </div>

    <div class="foo_footer">
      <div class="container">
        <div class="cont_flex">
          <div>
            <a href="#" class="sign_up">SIGN UP NOW!</a>
          </div>

          <div>
            <ul class="social">
              <li>
                <a href="">FOLLOW US</a>
              </li>
              <li>
                <a href="#"
                  ><img src="../assets/img/footer-facebook.png" alt="icon"
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img src="../assets/img/footer-twitter.png" alt="icon"
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img src="../assets/img/footer-youtube.png" alt="icon"
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img src="../assets/img/footer-pinterest.png" alt="icon"
                /></a>
              </li>
              <li>
                <a href="#"
                  ><img src="../assets/img/footer-periscope.png" alt="icon"
                /></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use "./../assets/style/partials/variables.scss" as *;
footer ul {
  list-style: none;
  line-height: 21px;
  a {
    cursor: pointer;
    color: grey;
    text-decoration: none;
    &:hover {
      color: rgb(180, 180, 180);
      text-decoration: underline;
    }
  }
}
.container {
  max-width: 1200px;
  margin: auto;
}
.nav_footer {
  background-color: #0282f9;
  height: 7rem;
  display: flex;
  align-items: center;
  color: white;
  .blu_nav {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 4rem;
    li {
      display: flex;
      align-items: center;
      gap: 0.5rem;
      white-space: nowrap;
      cursor: pointer;
      img {
        height: 2.4rem;
      }
      &:hover {
        font-weight: bold;
      }
    }
  }
}

.main_footer {
  background-image: url(../assets/img/footer-bg.jpg);
  color: white;
  height: 25rem;
  position: relative;
  overflow: hidden;
  img {
    height: 30rem;
    margin-left: 13rem;
    position: absolute;
    top: -33px;
    right: 21rem;
  }
}
.container-f {
  max-width: 1200px;
  margin: auto;
  display: flex;
  gap: 2rem;
  padding: 6rem 0;
  li:first-child {
    font-weight: bold;
    font-size: 1.1em;
  }
}
.first-column {
  li:nth-child(9) {
    font-weight: bold;
    font-size: 1.1em;
  }
}

.foo_footer {
  background-color: #303030;
  padding: 1rem 0;
  .cont_flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
    .sign_up {
      color: white;
      text-decoration: none;
      border: 1px solid #0282f9;
      padding: 0.6rem;
      &:hover {
        background-color: rgba(128, 128, 128, 0.5);
      }
    }
  }
}
.social {
  display: flex;
  align-items: center;
  gap: 1rem;
}
.social li:not(:first-child) a:hover {
  opacity: 0.5;
}
</style>
