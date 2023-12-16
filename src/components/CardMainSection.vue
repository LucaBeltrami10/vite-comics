<template lang="">
<article>
    <img :src="imageSrc" :alt="descriptionImage">
    <p>{{title}}</p>
</article>
</template>
<script>
export default {
    name: 'CardMainSection',
    props: [
        'imageSrc',
        'descriptionImage',
        'title',
    ],

}
</script>
<style lang="scss" scoped>
article {
    height: 140px;
    width: calc((100% / 6) - 16px);
    background-color: magenta;
    margin: 35px 8px 0 8px;

    img {
        width: 100%;
    }

    p {
        padding: 10px 0;
    }
}
</style>