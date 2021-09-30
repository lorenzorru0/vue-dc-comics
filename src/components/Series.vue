<template>
    <div class="series">
        <img :src="singleSeries.thumb" :alt="singleSeries.series">
        <p>{{singleSeries.series}}</p>
    </div>
</template>

<script>
export default {
    name: 'Series',
    props: ['singleSeries']
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

.series {
    width: $widthSeries;
    padding: 1.25rem .625rem;

    img {
        width: 100%;
        height: 11.25rem;
        object-fit: cover;
        object-position: top;
    }

    p {
        color: $white;
        text-transform: uppercase;
        margin-top: .625rem;
    }
}
</style>