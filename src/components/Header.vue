
<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in menu" :key="index">
            <a href="link.url" :class="{active : link.currentPage}">{{link.nameLink}}</a>
          </li>    
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      menu:[
        {
          nameLink: "CHARATCTERS",
          url: "#",
          currentPage: false
        },
         {
          nameLink: "COMICS",
          url: "#",
          currentPage: true
        },
         {
          nameLink: "MOVIES",
          url: "#",
          currentPage: false
        },
        {
          nameLink: "TV",
          url: "#",
          currentPage: false
        },
        {
          nameLink: "GAMES",
          url: "#",
          currentPage: false
        },
         {
          nameLink: "COLECTIBLES",
          url: "#",
          currentPage: false
        },
         {
          nameLink: "VIDIOS",
          url: "#",
          currentPage: false
        },
         {
          nameLink: "FANS",
          url: "#",
          currentPage: false
        },
        {
          nameLink: "NEWS",
          url: "#",
          currentPage: false
        },
         {
          nameLink: "SHOPS",
          url: "#",
          currentPage: false
        },
      ]
    }
  }
 
}
</script>


<style scoped lang="scss">
header{ 
  }
.container{
  @import'../assets/style/variables';
  max-width: $containerSize;
  margin: auto;
  padding-top: 1.875rem;
  display: flex;
  justify-content: space-between;
  align-items: end;
  
}
.logo{
  img{
    width: 80%;
  padding-bottom: .625rem;
  }
}
nav{
  ul{
  display: flex;
  list-style: none;
  
    li{
       padding: 0 .9375rem;
    }

    a{
      color: black;
      font-weight: 700;
      text-decoration: none ;
      // padding: .9375rem;
      display: inline-block;

       &.active{
         border-bottom:5px solid #0282f9;
         color: #4c95f9;
         padding-bottom: 2.5rem;
       }
    }
  }
}



</style>
