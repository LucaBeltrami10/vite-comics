<template>
    <main>
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
    color: $main-background;

    p {
        padding: 1rem 0;
    }
}
</style>