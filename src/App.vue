<template>
  <HeaderComponent />
  <main>main</main>
  <footer>footer</footer>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
export default {
  name: 'App',
  components: {
    HeaderComponent
  }
}
</script>

<style lang="scss" scoped>
main,
footer {
  font-family: 'Open Sans', sans-serif;
}
</style>
