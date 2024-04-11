<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                'Characters',
                'Comics',
                'Movies',
                'Tv',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop'
        ],
        activeItem: null
        }
    },
    methods: {
        activeLink(index){
            this.activeItem = index;
        }
    },
}

</script>

<template>
   <nav class="navbar navbar-expand-lg">
        <div class="container">
            <a class="navbar-brand" href="#">
                <img src="../assets/img/dc-logo.png" alt="dc-logo">
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item" v-for="link, index in links" @click="activeLink(index)">
                        <a class="nav-link active" :class="{'ms-active': index == activeItem}" aria-current="page" href="#">{{link}}</a>
                    </li>
                </ul>
            </div>
        </div>
   </nav>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;

    .nav-link{
        &.ms-active{
            color: $brand-primary;
            border-bottom: 5px solid $brand-primary;
        }
        &:hover{
            color: $brand-primary;
        }
    }
</style>