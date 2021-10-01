<template>
    <section :style="`background-image: url(${src});`">
    </section>
</template>

<script>
export default {
    name: 'SectionHero',
    props: ['src']
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

section {
    height: 20rem;
    background-size: cover;
}
</style>