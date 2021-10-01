<template>
  <section>
      <!-- Main top  -->
      <div class="main-top">
      <div class="container">
        <!-- <Card :key="index" v-for="(data, index) in myJson" :info="data"/> -->
      </div>  
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
// importo i nuovi contetnti in questo componento per farle funzionare qua
// import json from "./dc-comics.json";
// import Card from "./Card.vue"
export default {
  // components:{
  //   Card
  // },
  data(){
    return{
      // myJson: json,
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
  },
  name: 'Content',
}
</script>
<style scoped lang="scss">
.main-top{
  height: 100%;
  background-color: black;
}
.hero{  
  background-image:url("../assets/img/jumbotron.jpg");
  background-size: cover;
  height: 25rem;
}

.container{
    display: flex;
    flex-wrap: wrap;
    &.container{
      @import'../assets/style/variables';
      max-width: $containerSize;
      margin: auto;
      color: white;
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
