<script>
export default {
    name: 'AppInfo',
}
</script>

<template>
    <section class="ms-bg">
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <div class="col-5 d-flex gap-4">
                    <div>
                        <div class="text-white">
                            DC COMICS
                        </div>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                        </ul>
                        <div class="text-white">
                            SHOP
                        </div>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC collectibles</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <div class="text-white">
                            DC
                        </div>
                        <ul>
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy policy (New)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subdcription</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact Us</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <div class="text-white">
                            SITES
                        </div>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="ms-img-bg col-7"></div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    @use '../style/partials/variables' as *;
    section{
        &.ms-bg {
            background-image: url(../assets/img/footer-bg.jpg);
            background-size: cover;
            background-repeat: no-repeat;
        }
        .ms-img-bg {
            height: 400px;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position: center;
        }
        ul {
            a {
                font-size: .875rem;
                color: $brand-tertiary;
                &:hover {
                    color: $brand-primary;
                }
            }
        }
    }
    
</style>