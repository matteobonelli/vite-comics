<template>
    <header class="container my-4">
        <div class="d-flex justify-content-between align-items-center">
            <img src="../assets/images/dc-logo.png" alt="logo">
            <NavBar />
        </div>

    </header>
</template>

<script>
import NavBar from './header/NavBar.vue';
export default {
    name: 'HeaderComponent',
    components: {
        NavBar
    }
}
</script>

<style lang="scss" scoped>
header {
    font-family: 'Fira Sans Condensed', sans-serif;
}
</style>