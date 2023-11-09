<template>
  <HeaderComponent />
  <MainComponent />
  <footer>footer</footer>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent
  }
}
</script>

<style lang="scss" scoped>
main,
footer {
  font-family: 'Fira Sans Condensed', sans-serif;
}
</style>
