<template>
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
</template>

<script>
export default {
    name: 'BonusMain',

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

div.container {
    @include flex(row, space-between, center);
    background-color: $background-bonus;
    color: $color-bonus;

    article {
        @include flex(row, space-between, center);
        padding: 1.5rem 0;

        img {
            height: 40px;
        }

        p {
            margin-left: 0.5rem;
        }
    }
}
</style>