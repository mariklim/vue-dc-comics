<template>
  <section>
      <!-- Main top  -->
      <div class="main-top">

      </div>
      <!--/ Main top  -->

      <!-- Main bottom icons nav -->
      <div class="main-bottom">
        <div class="main-nav">
            <div class="link-icon">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="comics digital">
              <span>DIGITAL COMICS</span>
            </div>
            <div class="link-icon">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="comics digital">
              <span>DIGITAL COMICS</span>
            </div>
            <div class="link-icon">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="comics digital">
              <span>DIGITAL COMICS</span>
            </div>
            <div class="link-icon">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="comics digital">
              <span>DIGITAL COMICS</span>
            </div>
            <div class="link-icon">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="comics digital">
              <span>DIGITAL COMICS</span>
            </div>
        </div>
      </div>
      <!-- /Main bottom icons nav -->


  </section>
</template>

<script>
export default {
  name: 'Content',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main-top{  
  background-color: black;
  color: azure;
  height: 12.5rem;
}
.main-bottom{
  @import'../assets/style/variables';
  background-color: $mainColor;
    .main-nav{
      display: flex;
      @import'../assets/style/variables';
      max-width: $containerSize;
      margin: auto;
      color: white;
    }
    
    .link-icon{
      display: flex;
      align-items: center;
      padding: 1.875rem;
      width: calc(100% / 5);
        & img{
          width: 40%;
          margin-right: .9375rem;
        }
    }
}


</style>
