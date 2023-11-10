<template>
    <main>
        <div class="jumbo-container">
        </div>
        <div class="container main-content">
            <div class="row">
                <MainComics v-for="comic in comics" :thumb="comic.thumb" :series="comic.series" />
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
main {
    background-color: #1e1b18;
    color: white;

    .main-content {
        padding: 40px;
    }

    .jumbo-container {
        height: 400px;
        background-image: url('../assets/images/jumbotron.jpg')
    }



    ;
}
</style>