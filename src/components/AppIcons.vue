<script>
export default {
    name: 'AppIcons',
    data() {
        return {
            products: [
                {
                    text:'DIGITAL COMICS',
                    img:'buy-comics-digital-comics.png'
                },
                {
                    text:'DC MERCHANDISE',
                    img:'buy-comics-merchandise.png'
                },
                {
                    text:'SUBSCRIPTION',
                    img:'buy-comics-subscriptions.png'
                },
                {
                    text:'COMIC SHOP LOCATOR',
                    img:'buy-comics-shop-locator.png'
                },
                {
                    text:'DC POWER VISA',
                    img:'buy-dc-power-visa.svg'
                },
            ]
        }
    },
    methods: {
        generateImg(image){
            return new URL(`../assets/img/${image}`, import.meta.url).href
        }
    },
}
</script>

<template>
    <section>
        <div class="container p-5">
            <div class="row">
                <div v-for="product in products" class="col d-flex align-items-center">
                    <div class="image">
                        <img :src="generateImg(product.img)" :alt="product.text">
                    </div>
                    <a class="text-white ps-2" href="#">{{product.text}}</a>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    section{
        background-color: $brand-primary;
        .image{
            width: 3rem;
            height: 3rem;
            img{
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }
    }
</style>