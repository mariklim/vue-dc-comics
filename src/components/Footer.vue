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
      </div>
      <!-- /Footer menu -->
    </div>
    <div class="footer-bottom">
      <div class="footer-bottom-container">
        <button>
          SIGN-UP NOW!
        </button>
        <div class="social-CTA">
          <span>FOLLOW US</span>
          <span class="icons-social">
            <ul>
              <li><img src="../assets/img/footer-facebook.png" alt="facebook"></li>
              <li><img src="../assets/img/footer-facebook.png" alt="facebook"></li>
              <li><img src="../assets/img/footer-facebook.png" alt="facebook"></li>
              <li><img src="../assets/img/footer-facebook.png" alt="facebook"></li>
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.footer-top {
  background-image: url("../assets/img/footer-bg.jpg");
  & .footer-top-container {
    display: flex;
    @import "../assets/style/variables";
    max-width: $containerSize;
    margin: auto;
    color: white;
    padding: 2.5rem 0;

      & .col{
        padding: 0 1.25rem;
      }
  }
}
.footer-bottom{
  background-color: #303030;
    & .footer-bottom-container {
      display: flex;
      justify-content: space-between;
      @import "../assets/style/variables";
      max-width: $containerSize;
      margin: auto;
      color: white;
      padding: 2.5rem 0;

        & .social-CTA{
          display: flex;
          align-items: center;
        }

}

}
.icons-social{
  & ul{
    display: flex;
    padding: 0 1.25rem;
     & li{
       padding: 0 .625rem;
     }   

  }
}
</style>
