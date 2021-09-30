<template>
    <section>
        <div class="container">
            <div>
                <h2>CURRENT SERIES</h2>
            </div>

            <div class="seriesContainer">
                <Series v-for="(series, index) in seriesJson" :key="index" :single-series="series"/>
            </div>

            <div>
                <button>LOAD MORE</button>
            </div>
        </div>
    </section>
</template>

<script>
import json from './dc-comics.json';
import Series from './Series.vue';

export default {
    name: 'SectionSeries',
    components: {
        Series
    },
    data() {
        return {
            seriesJson: json
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

section {
    background-color: #1c1c1c;

    .container {
        position: relative;
        padding: 1.875rem 0;

        & > div:first-child {
            position: absolute;
            top: -1.90625rem;
            display: inline-block;
            padding: .9375rem 1.875rem;
            background-color: $commonBlue;
            color: $white;
        }

        .seriesContainer {
            @include dFlex;
            flex-wrap: wrap;
        }

        & > div:last-child {
            text-align: center;
        }

        button {
            border: none;
            background-color: $commonBlue;
            color: $white;
            font-weight: bold;
            padding: .625rem 2.7rem;
            cursor: pointer;
        }
    }    
}

</style>