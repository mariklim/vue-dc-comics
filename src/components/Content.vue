<template>
  <section>
      <!-- Main top  -->
      <div class="main-top">
        <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <!--/ Main top  -->

      <!-- Main bottom icons nav -->
      <div class="main-bottom">
        <div class="main-nav">
            <div v-for="(image,index) in gallery" :key="index" class="link-icon">
              <img :src="image.scr" alt="">
              <span>{{image.title}}</span>
            </div>
        </div>
      </div>
      <!-- /Main bottom icons nav -->


  </section>
</template>

<script>
export default {
  name: 'Content',
  data(){
    return{
      gallery:[
        {
        scr:require('../assets/img/buy-comics-digital-comics.png'),
        title:"DIGITAL COMICS",
        },
        {
        scr:require("../assets/img/buy-comics-merchandise.png"),
        title:"DC MERCHANDISE",
        },
        {
        scr:require("../assets/img/buy-comics-subscriptions.png"),
        title:"SUBSCRIPTION",
        },
        {
        scr:require("../assets/img/buy-comics-shop-locator.png"),
        title:"COMICS SHOP LOCATOR",
        },
        {
        scr:require("../assets/img/buy-dc-power-visa.svg"),
        title:"CD POWER VISA",
        },
      ],
    }
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main-top{  
  background-color: black;
  color: azure;
  height: 25rem;
  overflow: hidden;

    img{
      object-fit:contain;
    }
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
