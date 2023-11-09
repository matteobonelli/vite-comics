<template>
    <ul class="nav nav-underline">
        <li class="nav-item" v-for="(link, index) in navbar" :key="index">
            <a class="nav-link text-uppercase" :class="{ 'active': link.active }" :href="link.url">{{ link.text }}</a>
        </li>
    </ul>
</template>

<script>
export default {
    name: 'NavBar',
    data() {
        return {
            navbar: [
                {
                    text: 'Characters',
                    url: '#',
                    active: false
                },
                {
                    text: 'Comics',
                    url: '#',
                    active: true
                },
                {
                    text: 'Movies',
                    url: '#',
                    active: false
                },
                {
                    text: 'Tv',
                    url: '#',
                    active: false
                },
                {
                    text: 'Games',
                    url: '#',
                    active: false
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    active: false
                },
                {
                    text: 'Videos',
                    url: '#',
                    active: false
                },
                {
                    text: 'Fans',
                    url: '#',
                    active: false
                },
                {
                    text: 'News',
                    url: '#',
                    active: false
                },
                {
                    text: 'Shop',
                    url: '#',
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
a {
    color: black;
}

.nav-underline .nav-link.active {
    color: #0282f9 !important;
}
</style>