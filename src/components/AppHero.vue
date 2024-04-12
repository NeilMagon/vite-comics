<script>
export default {
    name: 'AppHero',
}
</script>

<template>
    <section class="hero">
        <img src="../assets/img/jumbotron.jpg" alt="">
        <div class="container">
            <button type="button" class="btn btn-primary ms-m">
                CURRENT SERIES
            </button>
        </div>
    </section>
    <section>
        
    </section>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    .hero{
        height: 25rem;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
        .ms-m{
            margin-top: -1.875rem;
        }
    }
</style>