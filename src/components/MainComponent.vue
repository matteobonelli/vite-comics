<template>
    <main>
        <div class="container main-content">
            <h2>--> Content goes here &lt;-- </h2>
        </div>
        <MainCatalog />
    </main>
</template>

<script>
import MainCatalog from './main/MainCatalog.vue';
export default {
    name: 'MainComponent',
    components: {
        MainCatalog
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
}
</style>