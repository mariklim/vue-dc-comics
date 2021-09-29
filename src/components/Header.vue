
<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <nav>
      <ul>
        <li>
          <a href="#">Link</a>
        </li>
             <li>
          <a href="#">Link</a>
        </li>
             <li>
          <a href="#">Link</a>
        </li>
             <li>
          <a href="#">Link</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
  display: flex;
  justify-content: space-around;
  align-items: center;
}

nav{
  ul{
  display: flex;
  list-style: none;
    a{
      text-decoration: none ;
      padding: 1.25rem;
    }
  }
}

</style>
