<script>
    export default{
        name: 'HeroContent',
        props: {
            cardInfo: Object
        },
        methods: {
            generateImage(name) {
                return new URL(`${name}`, import.meta.url).href
            }
        }
    }
</script>

<template>
    <div class="col-2 pt-5">
        <div class="img-container">
            <img :src="generateImage(cardInfo.thumb)" alt="cardInfo.series">
        </div>
        <div class="text text-white pt-3">{{ cardInfo.series }}</div>
    </div>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    .img-container{
        width: 150px;
        height: 150px;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
    .text{
        text-transform: uppercase;
    }
</style>