<script>
export default {
    name: 'AppHero',
}
</script>

<template>
    <section class="ms-black">
        <div class="container">
            <h1 class="ms-white">Content goes here</h1>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;
    .ms-black{
        background-color: $brand-secondary;
        height: 100px;
    }
    .ms-white{
        color: #fff;
    }
</style>