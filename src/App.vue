<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss" scoped>
main,
footer {
  font-family: 'Fira Sans Condensed', sans-serif;
}
</style>
