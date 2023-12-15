<template>
    <header>
        <div class="container">
            <div>
                <img src="../assets/img/dc-logo.png" alt="Logo DC">
            </div>
            <nav>
                <ul>
                    <li>characters</li>
                    <li>comics</li>
                    <li>movies</li>
                    <li>tv</li>
                    <li>games</li>
                    <li>collectibiles</li>
                    <li>videos</li>
                    <li>fans</li>
                    <li>news</li>
                    <li>shop</li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


div.container {
    @include flex(row, space-between, center);
    background-color: $header-background;

    div {
        height: 3.5rem;

        img {
            height: 100%;
        }
    }

    nav {
        ul {
            @include flex(row, space-between, center);

            li {
                padding: 1rem 0 1rem 0rem;
                margin-left: 1rem;
                font-weight: 600;
                text-transform: uppercase;
                color: $color-text-navbar;
                font-size: 0.8rem;
                border-bottom: 3px solid rgba($color: #000000, $alpha: 0);

                &:hover {
                    color: $color-text-navbar-hover;
                    border-bottom: 3px solid $color-text-navbar-hover;
                }
            }
        }
    }
}
</style>