<template lang="">
    <footer>
        <div class="upper-footer">
            <div class="container top">
                <div>
                    <article>
                        <h1>dc comics</h1>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </article>
                    <article>
                        <h1>shop</h1>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </article>
                </div>
                <article>
                    <h1>dc</h1>
                    <ul>
                        <li>Term Of Use</li>
                        <li>Privacy e policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </article>
                <article>
                    <h1>sites</h1>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </article>
            </div>
        </div>
        <div class="bottom-footer">
            <div class="container bottom">
                <button>sign-up now!</button>
                <div class="social">
                    <h1>follow us</h1>
                    <img src="../assets/img/footer-facebook.png" alt="facebook logo">
                    <img src="../assets/img/footer-twitter.png" alt="twitter logo">
                    <img src="../assets/img/footer-youtube.png" alt="youtube logo">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest logo">
                    <img src="../assets/img/footer-periscope.png" alt="periscope logo">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


footer {
    div.upper-footer {
        background-image: url('../assets/img/footer-bg.jpg');

        div.container.top {
            @include flex(row, start, start);
            background-image: url('../assets/img/dc-logo-bg.png');
            background-size: 22rem;
            background-position: right;
            background-repeat: no-repeat;

            h1 {
                text-transform: uppercase;
                font-size: 1rem;
                color: $color-footer-title-list;
                margin: 0.5rem 0 0.5rem 0;
            }

            ul {
                margin: 0 1rem 0 0;

                li {
                    font-size: 0.7rem;
                    margin: 0 0 0.2rem 0;
                    color: $color-footer-list-item;
                }
            }
        }
    }

    div.bottom-footer {
        background-color: $bottom-footer-background;

        div.container.bottom {
            @include flex(row, space-between, center);

            button {
                border: 2px solid $color-border-button;
                padding: 0.7rem;
                text-transform: uppercase;
                font-size: 0.7rem;
                color: white;
                background-color: rgba($color: #000000, $alpha: 0)
            }

            div.social {
                @include flex(row, start, center);

                h1 {
                    text-transform: uppercase;
                    color: $color-social-title;
                    font-size: 1rem;
                    margin-right: 1rem;
                }

                img {
                    width: 25px;
                    margin-right: 0.5rem;
                }
            }
        }
    }

}
</style>