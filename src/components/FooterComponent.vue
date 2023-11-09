<template>
    <footer>
        <section class="dc-bg py-4">
            <div class="container">
                <div class="row">
                    <div class="col-1">
                        <h5 class="text-uppercase">Dc Comics</h5>
                        <ul>
                            <li v-for="(link, index) in dcComics" :key="index">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                        <h5 class="text-uppercase">Shop</h5>
                        <ul>
                            <li v-for="(link, index) in shop" :key="index">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-1">
                        <h5 class="text-uppercase">Dc</h5>
                        <ul>
                            <li v-for="(link, index) in dc" :key="index">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-1">
                        <h5 class="text-uppercase">Sites</h5>
                        <ul>
                            <li v-for="(link, index) in sites" :key="index">
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-6 align-self-end">
                        <img src="../assets/images/dc-logo-bg.png" alt="dc-logo">
                    </div>
                </div>
            </div>
        </section>
        <FollowUsComponent />
    </footer>
</template>

<script>
import FollowUsComponent from './footer/FollowUsComponent.vue'
export default {
    name: 'FooterComponent',
    components: {
        FollowUsComponent
    },
    data() {
        return {
            dcComics: [
                {
                    text: 'Characters',
                    url: '#',
                    active: false
                },
                {
                    text: 'Comics',
                    url: '#',
                    active: false
                },
                {
                    text: 'Movies',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },
                {
                    text: 'Games',
                    url: '#',
                    active: false
                },
                {
                    text: 'Videos',
                    url: '#',
                    active: false
                },
                {
                    text: 'News',
                    url: '#',
                    active: false
                },
            ],
            shop: [
                {
                    text: 'Shop DC',
                    url: '#',
                    active: false
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                    active: false
                },
            ],
            dc: [
                {
                    text: 'Terms of Use',
                    url: '#',
                    active: false
                },
                {
                    text: 'Privacy policy(New)',
                    url: '#',
                    active: false
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                    active: false
                },
                {
                    text: 'Advertising',
                    url: '#',
                    active: false
                },
                {
                    text: 'Jobs',
                    url: '#',
                    active: false
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                    active: false
                },
                {
                    text: 'Talent Workshops',
                    url: '#',
                    active: false
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                    active: false
                },
                {
                    text: 'Ratings',
                    url: '#',
                    active: false
                },
                {
                    text: 'Shop Help',
                    url: '#',
                    active: false
                },
                {
                    text: 'Contact Us',
                    url: '#',
                    active: false
                },
            ],
            sites: [
                {
                    text: 'DC',
                    url: '#',
                    active: false
                },
                {
                    text: 'MAD Magazine',
                    url: '#',
                    active: false
                },
                {
                    text: 'DC Kids',
                    url: '#',
                    active: false
                },
                {
                    text: 'DC Universe',
                    url: '#',
                    active: false
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.dc-bg {
    background-image: url('../assets/images/footer-bg.jpg');
    background-size: cover;
}

.container {
    position: relative;
}

h5 {
    color: white;
}

img {
    background-size: cover;
}

ul {
    padding: 0;
    font-family: 'Open Sans', sans-serif;

    a {
        color: #959595;
        text-decoration: none;
        font-size: 12px;
    }
}
</style>