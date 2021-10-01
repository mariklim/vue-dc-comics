<template>
  <div>
      <img :src="info.thumb" alt="info.type">
      <p>{{info.series}}</p>
  </div>
</template>

<script>
export default {
    name: "Card",
    props:["info"]
}
</script>

<style>

</style>