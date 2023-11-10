<template>
    <main>
        <div class="jumbo-container">
        </div>
        <div class="container main-content">
            <button class="btn current-series text-uppercase">Current series</button>
            <div class="row mt-3">
                <MainComics v-for="comic, index in comics" :thumb="comic.thumb" :series="comic.series" :key="index" />
            </div>
            <div class="d-flex justify-content-center">
                <button class="btn text-uppercase">Load more</button>
            </div>
        </div>


        <MainCatalog />
    </main>
</template>

<script>
import MainCatalog from './main/MainCatalog.vue';
import MainComics from './main/MainComics.vue'
import { comicsList } from './data/data'
export default {
    name: 'MainComponent',
    components: {
        MainCatalog,
        MainComics
    },
    data() {
        return {
            comics: comicsList
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

main {
    background-color: #1e1b18;
    color: white;

    .main-content {
        padding: 40px;
        position: relative;

        .current-series {
            position: absolute;
            top: -25px;
            width: 15%;
            font-size: 24px;
        }
    }

    .jumbo-container {
        height: 400px;
        background-image: url('../assets/images/jumbotron.jpg')
    }

    .btn {
        background-color: $brand_primary;
        color: white;
        font-size: 20px;
        border-radius: 0;
        width: 250px;
    }
}
</style>