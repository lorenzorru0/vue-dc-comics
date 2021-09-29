<template>
    <section>
        <div class="container">
            <p>--> Content goes here</p>
        </div>
    </section>
</template>

<script>
export default {
    name: 'SectionMistery'
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

section {
    @include dFlex;
    align-items: center;
    height: 12.5rem;
    background-color: #000;
    color: #fff;
}

</style>