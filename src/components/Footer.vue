<template>
  <footer>
    <div class="footer-top">
      <!-- Footer menu -->
      <div class="footer-top-container">
        <div class="col">
          <h2>DC COMICS</h2>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>

          <h2>DC SHOP</h2>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
          </ul>
        </div>

        <div class="col">
          <h2>DC</h2>
          <ul>
            <li>Terms Of Use</li>
            <li>Privacy Policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>

        </div>
        <div class="col">
          <h2>SITES</h2>
          <ul>
            <li>DC</li>
            <li>DC UNIVERSE INFINITE</li>
            <li>DC Kids</li>
            <li>DC Shop</li>
            <li>MAD Magazine</li>
          </ul>
        </div>
      </div>
      <!-- /Footer menu -->
    </div>
    <div class="footer-bottom">
      <div class="footer-bottom-container">
        <button class="signUp">SIGN-UP NOW!</button>
        <div class="social-CTA">
          <span>FOLLOW US</span>
          <span class="icons-social">
            <ul>
              <li>
                <img src="../assets/img/footer-facebook.png" alt="facebook" />
              </li>
              <li>
                <img src="../assets/img/footer-facebook.png" alt="facebook" />
              </li>
              <li>
                <img src="../assets/img/footer-facebook.png" alt="facebook" />
              </li>
              <li>
                <img src="../assets/img/footer-facebook.png" alt="facebook" />
              </li>
            </ul>
          </span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../assets/style/variables";
.footer-top {
  background-image: url("../assets/img/footer-bg.jpg");
  & .footer-top-container {
    display: flex;
    max-width: $containerSize;
    margin: auto;
    color: white;
    padding: 2.5rem 0;
    & .col {
      padding: 0 1.25rem;
      & h2{
        margin-bottom: .625rem;
      }
      & li{
        font-size: .8125rem;
        color: gray;
      }
    }
  }
}


.footer-bottom {
  background-color: $gray;
  & .footer-bottom-container {
    display: flex;
    justify-content: space-between;
    @import "../assets/style/variables";
    max-width: $containerSize;
    margin: auto;
    color: white;
    padding: 2.5rem 0;

    & .social-CTA {
      display: flex;
      align-items: center;
    }
    & .signUp{
       background: transparent;
       border: 2px solid $mainColor;
       color: white;
       padding: .4375rem 1.25rem;
       font-size: 1.0625rem;
    }
  }
}
.icons-social {
  & ul {
    display: flex;
    padding: 0 1.25rem;
    & li {
      padding: 0 0.625rem;
    }
  }
}
</style>
