<template>
    <main>
        <div class="jumbotron"></div>
        <div class="container">
            <p>--- CONTENUTO ---</p>
        </div>

    </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

main {
    background-color: $main-background;

    div.jumbotron {
        height: 280px;
        width: 100%;
        background-image: url(../assets/img/jumbotron.jpg);
        background-position: top;
        background-repeat: no-repeat;
        background-size: 100%;
    }

    p {
        padding: 1rem 0;
        color: white;
    }
}
</style>