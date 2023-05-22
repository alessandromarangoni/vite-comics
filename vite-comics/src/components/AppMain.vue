<script>
export default {
    name: "AppMain",
    props: ["items"]
}
</script>

<template>
    <div class="appMain">

        <div class="container">
            <div class="row">
                <div class="col-11 d-flex flex-wrap justify-content-between mb-3">
                    <template v-for="item in items" class="">
                        <div class="item_card my-5">
                            <img class="" :src="item.thumb" alt="">
                            <p class="mt-3 text-white">{{ item.series }}</p>
                        </div>
                    </template>
                </div>
            </div>
        </div>
        <button class="btn btn-primary px-5 mb-3">load more</button>
    </div>
</template>

<style scoped lang="scss">
.appMain {
    background-color: rgba(0, 0, 0, 0.85);
    text-align: center;
}

.row {
    justify-content: center;
}

.item_card {
    width: 180px;
    height: 180px;

    & :hover {
        transform: scale(1.05);
    }

    img {
        width: 180px;
        height: 180px;
        object-fit: cover
    }

    p {
        text-align: center;
        line-break: auto;
        font-size: small
    }

    ;
}
</style>