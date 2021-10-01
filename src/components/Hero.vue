<template>
    <section :style="`background-image: url(${src});`">
    </section>
</template>

<script>
export default {
    name: 'Hero',
    props: ['src']
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
section {
    height: 20rem;
    background-size: cover;
}
</style>