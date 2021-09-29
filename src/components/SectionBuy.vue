<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(element, index) in elements" :key="index" >
                    <img :src="'../imgMain/' + element.src" :alt="element.name">
                    <span>{{element.name}}</span>
                </li>
            </ul> 
        </div>
    </section>
</template>

<script>
export default {
    name: 'SectionBuy',
    data() {
        return {
            elements: {
                digitalComics: {
                    name: 'DIGITAL COMICS',
                    src: 'buy-comics-digital-comics.png',
                    link: '#',
                    active: false
                },
                dcMerchandise: {
                    name: 'DC MERCHANDISE',
                    src: 'buy-comics-merchandise.png',
                    link: '#',
                    active: false
                },
                subscription: {
                    name: 'SUBSCRITION',
                    src: 'buy-comics-subscriptions.png',
                    link: '#',
                    active: false
                },
                comicShopLocator: {
                    name: 'DIGITAL COMICS',
                    src: 'buy-comics-shop-locator.png',
                    link: '#',
                    active: false
                },
                dcPowerVisa: {
                    name: 'DC POWER VISE',
                    src: 'buy-dc-power-visa.svg',
                    link: '#',
                    active: false
                },
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

section {
    background-color: $commonBlue;

    ul {
        @include dFlex;
        justify-content: space-evenly;
        @include list;
        padding: 4rem 0;

        li {
            @include dFlex;
            align-items: center;
            color: #fff;

            img {
                height: 4rem;
                margin-right: .625rem;
            }

            &:last-child img {
                height: 3rem;
            }
        }
    }
}

</style>