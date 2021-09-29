<template>
    <footer>
        <div class="footerTop">
            <div class="container">
                <nav>
                    <div>
                        <ul>
                            <li> <h3>DC COMICS</h3> </li>
                            <li> <a href="">Characters</a> </li>
                            <li> <a href="">Comics</a> </li>
                            <li> <a href="">Movies</a> </li>
                            <li> <a href="">TV</a> </li>
                            <li> <a href="">Games</a> </li>
                            <li> <a href="">Videos</a> </li>
                            <li> <a href="">News</a> </li>
                            <li> <h3>SHOP</h3> </li>
                            <li> <a href="">Shop DC</a> </li>
                            <li> <a href="">Shop DC Collectibles</a> </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li> <h3>DC</h3> </li>
                            <li> <a href="">Term Of Use</a> </li>
                            <li> <a href="">Privacy policy (New)</a> </li>
                            <li> <a href="">Ad Choices</a> </li>
                            <li> <a href="">Advertising</a> </li>
                            <li> <a href="">Jobs</a> </li>
                            <li> <a href="">Subscriptions</a> </li>
                            <li> <a href="">Talent Workshops</a> </li>
                            <li> <a href="">CPSC Certificates</a> </li>
                            <li> <a href="">Ratings</a> </li>
                            <li> <a href="">Shop Help</a> </li>
                            <li> <a href="">Contact Us</a> </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li> <h3>SITES</h3> </li>
                            <li> <a href="">DC</a> </li>
                            <li> <a href="">MAD Magazine</a> </li>
                            <li> <a href="">DC Kids</a> </li>
                            <li> <a href="">DC Universe</a> </li>
                            <li> <a href="">DC Power Visa</a> </li>
                        </ul>
                    </div>
                </nav>

                <div>
                    <!-- <img src="../assets/img/dc-logo-bg-png" alt="Logo Footer Top"> -->
                </div>
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
    name: 'Footer'
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/variables.scss';

footer {
    .footerTop {
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: contain;
        padding: {
            top: 1.875rem;
            bottom: 3.125rem;
        };
        
        .container {
            @include dFlex;
        }

        nav {
            @include dFlex;

            div {
                margin-right: 1.75rem;
            }

            ul {
                @include list;

                h3 {
                    color: #fff;
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
                color: #fff;
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