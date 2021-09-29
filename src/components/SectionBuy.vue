<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(element, index) in elements" :key="index" >
                    <img :src="'../../public/img/' + element.src + '.png'" :alt="element.name">
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
                    src: 'buy-comics-digital-comics',
                    link: '#',
                    active: false
                },
                dcMerchandise: {
                    name: 'DC MERCHANDISE',
                    src: 'buy-comics-merchandise',
                    link: '#',
                    active: false
                },
                subscription: {
                    name: 'SUBSCRITION',
                    src: 'buy-comics-subscriptions',
                    link: '#',
                    active: false
                },
                comicShopLocator: {
                    name: 'DIGITAL COMICS',
                    src: 'buy-comics-shop-locator',
                    link: '#',
                    active: false
                },
                dcPowerVisa: {
                    name: 'DC POWER VISE',
                    src: 'buy-dc-power-visa',
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
        @include list;

        li {
            @include dFlex;
        }
    }
}

</style>