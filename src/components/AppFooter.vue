<template lang="">
    <footer>
        <div class="container">

            <div class="upper-footer">
                <div class="ul-container">
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

                <div class="img-container">

                </div>

            </div>

            <div class="bottom-footer">

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
    background-image: url('../assets/img/footer-bg.jpg');
}

div.container {
    @include flex(row, space-between, center);
    background-image: url('../assets/img/dc-logo-bg.png');
    background-size: 22rem;
    background-position: right;
    background-repeat: no-repeat;

    div.upper-footer {


        div.ul-container {
            @include flex(row, start, start);
            width: 100%;


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
}
</style>