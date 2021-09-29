<template>
    <header class="container">
        <div>
            <img src="../assets/img/dc-logo.png" alt="Logo image">
        </div>
        <div>
            <ul>
                <li v-for="(element, index) in nav" :key="index"> <a :class="{active : element.active}" :href="element.link">{{element.name}}</a> </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            nav: {
                characters: {
                    name: 'CHARACTERS',
                    link: '#',
                    active: false
                },
                comics: {
                    name: 'COMICS',
                    link: '#',
                    active: true
                },
                movies: {
                    name: 'MOVIES',
                    link: '#',
                    active: false
                },
                tv: {
                    name: 'TV',
                    link: '#',
                    active: false
                },
                games: {
                    name: 'GAMES',
                    link: '#',
                    active: false
                },
                collectibles: {
                    name: 'COLLECTIBLES',
                    link: '#',
                    active: false
                },
                videos: {
                    name: 'VIDEOS',
                    link: '#',
                    active: false
                },
                fans: {
                    name: 'FANS',
                    link: '#',
                    active: false
                },
                news: {
                    name: 'NEWS',
                    link: '#',
                    active: false
                },
                shop: {
                    name: 'SHOP',
                    link: '#',
                    active: false
                }
            }
            }
            
    }
}
</script>

<style lang="scss" scoped>
@import url(../assets/scss/variables.scss);

header {
    display: flex;
    align-items: center;
    justify-content: space-between;

    img {
        width: 5rem;
    }

    ul {
        display: flex;
        list-style: none;

        li {
            padding: 0 .9375rem;
        }

        a {
            display: inline-block;
            text-decoration: none;
            color: #000;
            padding: 3.125rem 0;

            &.active {
                color: $commonBlue;
                border-bottom: .4375rem solid $commonBlue;
            }
        }
    }
}
</style>