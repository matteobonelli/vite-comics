<template>
    <div class="catalog-bg">
        <div class="container">
            <ul class="nav d-flex justify-content-between align-items-center">
                <li class="nav-item" v-for="(link, index) in catalog" :key="index">
                    <div class="d-flex align-items-center">
                        <img :src="link.image" :alt="link.text">
                        <a class="nav-link text-uppercase" :href="link.url">{{ link.text }}</a>

                    </div>

                </li>
            </ul>
        </div>

    </div>
</template>

<script>
export default {
    name: 'MainCatalog',
    data() {
        return {
            catalog: [
                {
                    text: 'Digital Comics',
                    image: '/images/buy-comics-digital-comics.png',
                    url: '#',
                    active: false
                },
                {
                    text: 'DC Merchandise',
                    image: '/images/buy-comics-merchandise.png',
                    url: '#',
                    active: false
                },
                {
                    text: 'Subscription',
                    image: '/images/buy-comics-subscriptions.png',
                    url: '#',
                    active: false
                },
                {
                    text: 'Comic Shop Locator',
                    image: '/images/buy-comics-shop-locator.png',
                    url: '#',
                    active: false
                },
                {
                    text: 'Dc Power Visa',
                    image: '/images/buy-dc-power-visa.svg',
                    url: '#',
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.catalog-bg {
    background-color: #0282f9;
    padding: 40px;
    font-family: 'Open Sans', sans-serif;
    position: relative;
    z-index: 10;
}

a {
    color: white;

    &:hover {
        color: white;
        text-decoration: underline;
    }
}

img {
    width: 60px;
    height: 70%;
    padding-right: 10px;
}
</style>