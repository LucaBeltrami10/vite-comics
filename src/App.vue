<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import app

export default {
    components: {
        AppHeader,
        AppMain,
    }
}

</script>

<template>
    <AppHeader />
    <AppMain />
</template>

<style lang="scss">
@use '../src/styles/general.scss' as *;
</style>
