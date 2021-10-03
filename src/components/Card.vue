<template>
<div class="cards-container">
     <div class="cover-img">
        <img :src="info.thumb" :alt="info.series">
     </div>
         <p>{{info.series}}</p>
 </div> 
</template>

<script>
export default {
    name: "Card",
    props:["info"]
}
</script>

<style lang="scss">
 @import '../assets/style/variables';
 .cards-container{
    width: calc($containerSize / 6);}
    .cover-img{
      width: calc($containerSize / 6);
      height: 12.5rem;
      overflow: hidden;
      padding: .9375rem;
      margin-bottom: .625rem;

       img {
           width: 100%;
       }
}
</style>