<template>
    <div class="col-12 col-md-2 mb-4">
        <img :src="thumb" :alt="series" class="mb-3">
        <h5 class="text-uppercase">{{ series }}</h5>
    </div>
</template>

<script>
export default {
    name: 'MainComics',
    props: {
        thumb: String,
        series: String
    }
}
</script>

<style lang="scss" scoped>
h5 {
    color: white;
}

img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    object-position: top;
}
</style>