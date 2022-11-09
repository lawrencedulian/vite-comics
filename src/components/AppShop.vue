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
                    image: "buy-comics-subscriptions",
                    title: "subscriptions",
                },
                {
                    image: "buy-comics-shop-locator.png",
                    title: "comic shop locator",
                },
                {
                    image: "buy-comics-visa.png",
                    title: "dc power visa",
                }
            ]
        }
    }
}
</script>

<template>
    <div class="shops">
        <div class="shops-container">
            <ul>
                <li v-for="(shop, index) in shops" :key="index">
                    <img src="../assets/img/${shop.image}" alt="">
                    <p>{{ shop.title }}</p>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
.shops {
    width: 100%;
    height: 250px;

    background-color: #0282F9;
}
</style>