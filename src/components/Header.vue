
<template>
  <header>
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.25rem 2.5rem;
}

nav{
  ul{
  display: flex;
  list-style: none;
    a{
      color: black;
      font-weight: 700;
      text-decoration: none ;
      padding: .9375rem;
      display: inline-block;
       &.active{
         border-bottom:2px solid #0282f9;
         color: #4c95f9;
       }
    }
  }
}



</style>
