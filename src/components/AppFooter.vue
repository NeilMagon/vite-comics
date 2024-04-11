<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <section>
        <div class="container">
            <div class="d-flex justify-content-between align-items-center py-4">
                <div>
                    <button>SIGN-UP-NOW</button>
                </div>
                <div class="d-flex align-items-center">
                    <div class="text-white">FOLLOW US</div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    section{
        background-color: $brand-secondary-light;
    }
</style>