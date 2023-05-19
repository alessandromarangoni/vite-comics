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
        <section>

        </section>
    </div>
</template>
<style scoped>
.sec1_c {
    min-height: 150px;
}

.buy_image {
    height: 40px;
}

.text_sec1_container {
    font-size: small;
}
</style>