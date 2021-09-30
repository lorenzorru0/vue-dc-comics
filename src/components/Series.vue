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

.series {
    width: calc(100% / 6);
    padding: 1.25rem .625rem;

    img {
        width: 100%;
        height: 11.25rem;
        object-fit: cover;
        object-position: top;
    }

    p {
        color: #fff;
        text-transform: uppercase;
        margin-top: .625rem;
    }
}
</style>