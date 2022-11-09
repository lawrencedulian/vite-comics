<script>
export default {
    name: "AppShop",
    data() {
        return {
            shops: [
                {
                    image: "buy-comics-digital-comics.png",
                    title: "digital comics",
                },
                {
                    image: "buy-comics-merchandise.png",
                    title: " dc merchandise",
                },
                {
                    image: "buy-comics-subscriptions.png",
                    title: "subscriptions",
                },
                {
                    image: "buy-comics-shop-locator.png",
                    title: "comic shop locator",
                },
                {
                    image: "buy-dc-power-visa.svg",
                    title: "dc power visa",
                }
            ]
        }
    },
    methods: {
        getImageUrl(url) {
            return new URL(url, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="shops">
        <div class="shop-container">
            <ul class="shop-list">
                <li v-for="(shop, index) in shops" :key="index">
                    <img :src="getImageUrl(`../assets/img/${shop.image}`)" alt="">
                    <p>{{ shop.title.toUpperCase() }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
.shop-container {
    width: 80%;

    display: flex;
    justify-content: center;
}

.shop-list {
    display: flex;

    li {
        padding: .5em;

        display: flex;
        align-items: center;
    }

    img {
        width: 60px;
        height: 60px;
    }

    p {
        font-size: .8rem;
        margin: .8em;
        color: white;
    }
}
</style>