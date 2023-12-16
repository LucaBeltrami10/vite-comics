<template lang="">
<article>
    <div>
        <img :src="imageSrc" :alt="descriptionImage">
    </div>
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
    width: calc((100% / 6) - 16px);
    margin: 35px 8px 0 8px;

    div {
        width: 100%;
        height: 150px;
        overflow: hidden;
    }

    img {
        width: 100%;
    }

    p {
        padding: 10px 0;
        font-size: 0.6rem;
        color: white;
        text-transform: uppercase;
    }
}
</style>