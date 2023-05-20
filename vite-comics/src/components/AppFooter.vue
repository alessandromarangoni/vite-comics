<script>
export default {
    name: "AppFooter",
    data() {
        return {
            topFooterItems: [
                {
                    immagine: "/src/assets/buy-comics-digital-comics.png",
                    Text: "DIGGITAL COMICS"
                },
                {
                    immagine: "/src/assets/buy-comics-merchandise.png",
                    Text: "DIGGITAL "
                },
                {
                    immagine: "/src/assets/buy-comics-shop-locator.png",
                    Text: "DIGGITAL COMICS"
                },
                {
                    immagine: "/src/assets/buy-comics-subscriptions.png",
                    Text: "DIGGITAL COMICS"
                },
                {
                    immagine: "/src/assets/buy-dc-power-visa.svg",
                    Text: "DIGGITAL COMICS"
                }
            ],
            bottom_footer_dc_comics: [
                "Characters",
                "Comics",
                "Mavior",
                "Games",
                "Videos",
                "News",
            ],
            bottom_footer_dc: [
                "Terms Of Use",
                "Privacy policy(New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshops",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                " Contact Us",
            ],
            bottom_footer_sites: [
                "DE",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa",
            ],
            social_footer_icon: [
                "/src/assets/footer-facebook.png",
                "/src/assets/footer-twitter.png",
                "/src/assets/footer-youtube.png",
                "/src/assets/footer-pinterest.png",
                "/src/assets/footer-periscope.png",
            ]

        }
    }
}
</script>

<template>
    <div class="bg-primary">
        <section>
            <div class="container">
                <div class="row">
                    <div
                        class="col-12 d-flex justify-content-between align-items-center sec1_c flex-wrap flex-md-no-wrap gap-2">
                        <template v-for="item in topFooterItems" class="items_container">
                            <div class="pt-auto">
                                <img :src="item.immagine" alt="" class="img-fluid buy_image">
                                <span class="ps-3 text-white text_sec1_container">{{ item.Text }}</span>
                            </div>
                        </template>
                    </div>
                </div>
            </div>
        </section>
        <!-- parte main del footer -->
        <section class="bg_image">
            <div class="container">
                <div class="row">
                    <div class="col-6">
                        <div class="row pt-3 d-flex flex-wrap">
                            <div class="col-4">
                                <h3 class="ps-4 ms-1">dc comics</h3>
                                <ul v-for="item in bottom_footer_dc_comics">
                                    <li>{{ item }}</li>
                                </ul>
                                <h3 class=" mt-5 ps-4 ms-1">dc</h3>
                                <ul>
                                    <li>Shop DE Shop</li>
                                    <li class="pt-3">DC Collectibles</li>
                                </ul>
                            </div>
                            <div class="col-4">
                                <h3 class="ps-4 ms-1">sites</h3>
                                <ul v-for="item in bottom_footer_dc">
                                    <li>{{ item }}</li>
                                </ul>
                            </div>
                            <div class="col-4">
                                <h3 class="ps-4 ms-1">shop</h3>
                                <ul v-for="item in bottom_footer_sites">
                                    <li>{{ item }}</li>
                                </ul>
                            </div>
                        </div>
                    </div>

                    <div class="col-6 bg_logo">
                    </div>
                </div>
            </div>
        </section>
        <section>
            <div class="container">
                <div class="row">
                    <div class="col d-flex justify-content-between h_100px align-items-center">
                        <div><button>SING-UP NOW</button></div>
                        <div class="d-flex align-items-center">
                            <span class="">FOLLOW NOW</span>
                            <template v-for="item in social_footer_icon" class="">
                                <img :src="item" alt="social_logo" class="px-2">
                            </template>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
.h_100px {
    height: 100px;
}

.sec1_c {
    min-height: 150px;
}

ul li {
    list-style: none;
    line-height: 0.8rem;
    color: #ffffff7a
}

.bg_image {
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.col-4 h3 {
    text-transform: uppercase;
    color: white;
    padding: 1rem 0;
}

.buy_image {
    height: 40px;
}

.bg_logo {
    background-image: url(../assets/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position-y: center;
}

.text_sec1_container {
    font-size: small;
}
</style>