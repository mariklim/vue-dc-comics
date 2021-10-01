<template>
<div>
  <div class="card">
      <img  :src="info.thumb" alt="info.type">
      <p>{{info.series}}</p>
  </div>
</div>
</template>

<script>
export default {
    name: "Card",
    props:["info"]
}
</script>

<style scoped lang="scss">
.card{
    width: calc((100% / 6) - 1.875rem);
    padding: .625rem;
    
     & img{
        
     }
}

</style>