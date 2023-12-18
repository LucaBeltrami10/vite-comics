<template>
    <div>
        <div class="container">
            <article>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>digital comics</p>
            </article>
            <article>
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <p>dc merchandise</p>
            </article>
            <article>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <p>subscription</p>
            </article>
            <article>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <p>comic shop locator</p>
            </article>
            <article>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                <p>dc power visa</p>
            </article>

        </div>

    </div>
</template>

<script>
export default {
    name: 'BonusMain',

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

div {
    background-color: $background-bonus;

    div.container {
        @include flex(row, space-between, center);

        color: $color-bonus;

        article {
            @include flex(row, space-between, center);
            padding: 2.5rem 0;

            img {
                height: 40px;
            }

            p {
                margin-left: 0.5rem;
                text-transform: uppercase;
                font-size: 0.8rem;
            }
        }
    }

}
</style>