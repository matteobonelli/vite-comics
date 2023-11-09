<template>
    <section class="d-flex">
        <div class="container d-flex justify-content-between align-items-center">
            <button class="btn text-uppercase">Sign-up Now!</button>
            <ul class="nav align-items-center">
                <li class="text-uppercase nav-item me-4">Follow Us</li>
                <li v-for="(social, index) in socials" class="nav-item me-3" :key="index">
                    <img :src="social.image" alt="social">
                </li>
            </ul>
        </div>

    </section>
</template>

<script>
export default {
    name: 'FollowUsComponent',
    data() {
        return {
            socials: [
                {
                    image: '/images/footer-facebook.png'
                },
                {
                    image: '/images/footer-twitter.png'
                },
                {
                    image: '/images/footer-youtube.png'
                },
                {
                    image: '/images/footer-pinterest.png'
                },
                {
                    image: '/images/footer-periscope.png'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
section {
    background-color: #303030;
    padding: 35px 0px;
    position: relative;
    z-index: 10;

    .btn {
        color: white;
        font-size: 20px;
        border: 2px solid #0282f9;
        border-radius: 0;
    }
}

ul {
    list-style: none;
    font-size: 20px;

    .text-uppercase {
        color: #0282f9
    }
}
</style>