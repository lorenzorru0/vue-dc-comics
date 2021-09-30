<template>
    <footer>
        <div class="footerTop">
            <div class="container">
                <nav>
                    <div>
                        <ul>
                            <li> <h3>DC COMICS</h3> </li>
                            <li v-for="(link, index) in links.dcComics" :key="index"> <a :href="link.href">{{link.name}}</a> </li>
                            <li> <h3>SHOP</h3> </li>
                            <li v-for="(link, index) in links.shop" :key="index"> <a :href="link.href">{{link.name}}</a> </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li> <h3>DC</h3> </li>
                            <li v-for="(link, index) in links.dc" :key="index"> <a :href="link.href">{{link.name}}</a> </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li> <h3>SITES</h3> </li>
                            <li v-for="(link, index) in links.sites" :key="index"> <a :href="link.href">{{link.name}}</a> </li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>

        <div class="footerBottom">
            <div class="container">
                <div>
                    <button>SIGN-UP NOW!</button>
                </div>
                <div>
                    <h3>FOLLOW US</h3>
                    <a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook icon"></a>
                    <a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter icon"></a>
                    <a href="#"><img src="../assets/img/footer-youtube.png" alt="You Tube icon"></a>
                    <a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest icon"></a>
                    <a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope icon"></a>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            links: {
                dcComics: [
                    {
                        name: 'Characters',
                        href: '#' 
                    },
                    {
                        name: 'Comics',
                        href: '#' 
                    },
                    {
                        name: 'Movies',
                        href: '#' 
                    },
                    {
                        name: 'TV',
                        href: '#' 
                    },
                    {
                        name: 'Games',
                        href: '#' 
                    },
                    {
                        name: 'Videos',
                        href: '#' 
                    },
                    {
                        name: 'News',
                        href: '#' 
                    }
                ],
                shop: [
                    {
                        name: 'Shop DC',
                        href: '#' 
                    },
                    {
                        name: 'Shop DC Collectibles',
                        href: '#' 
                    }
                ],
                dc: [
                    {
                        name: 'Term Of Use',
                        href: '#' 
                    },
                    {
                        name: 'Privacy policy (New)',
                        href: '#' 
                    },
                    {
                        name: 'Ad Choices',
                        href: '#' 
                    },
                    {
                        name: 'Advertising',
                        href: '#' 
                    },
                    {
                        name: 'Jobs',
                        href: '#' 
                    },
                    {
                        name: 'Subscriptions',
                        href: '#' 
                    },
                    {
                        name: 'Talent Workshops',
                        href: '#' 
                    },
                    {
                        name: 'CPSC Certificates',
                        href: '#' 
                    },
                    {
                        name: 'Ratings',
                        href: '#' 
                    },
                    {
                        name: 'Shop Help',
                        href: '#' 
                    },
                    {
                        name: 'Contact Us',
                        href: '#' 
                    },
                ],
                sites: [
                    {
                        name: 'DC',
                        href: '#' 
                    },
                    {
                        name: 'MAD Magazine',
                        href: '#' 
                    },
                    {
                        name: 'DC Kids',
                        href: '#' 
                    },
                    {
                        name: 'DC Universe',
                        href: '#' 
                    },
                    {
                        name: 'DC Power Visa',
                        href: '#' 
                    },
                ]
            }
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: contain;

    .footerTop {
        .container {
            @include dFlex;
            padding: {
                top: 1.875rem;
                bottom: 3.125rem;
            };
            background-image: url('../assets/img/dc-logo-bg.png');
            background-position: 39.875rem -5.625rem;
            background-repeat: no-repeat;
        }

        nav {
            @include dFlex;

            div {
                margin-right: 1.75rem;
            }

            ul {
                @include list;

                h3 {
                    color: $white;
                    padding: 20px 0;
                }

                a {
                    @include link;
                    color: #959595;
                }
            }
        }

        img {
            width: 31.25rem;
        }
    }

    .footerBottom {
        background-color: #303030;
        padding: 1.875rem 0;

        .container {
            @include dFlex;
            align-items: center;
            justify-content: space-between;

            button {
                border: none;
                padding: .625rem;
                border: 2px solid $commonBlue;
                background-color: inherit;
                color: $white;
                cursor: pointer;
            }

            div:last-child {
                @include dFlex;
                align-items: center;

                h3 {
                    color: $commonBlue;
                }

                a {
                    display: inline-block;
                    margin-left: .9375rem;
                    border-radius: 50%;
                    

                    img {
                        display: block;
                    }
                }
            }
        }
    }
}

</style>