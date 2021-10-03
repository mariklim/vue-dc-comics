<template>
  <section :style="`background-image: url(${src});`">
    <div class="title-box">CURRENT SERIES</div>
  </section>
</template>

<script>
export default {
  name: "Hero",
  props: ["src"],
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
section {
  height: 20rem;
  background-size: cover;
  position: relative;
  & .title-box {
    background-color: $mainColor;
    color: white;
    font-size: 1.5625rem;
    font-weight: bold;
    display: inline-block;
    padding: 0.625rem 1.875rem;
    position: relative;
    top: 90%;
    left: 12%;
  }
}
</style>