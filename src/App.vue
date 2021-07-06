<template>
  <div id="app">
    <Navbar></Navbar>
    <Banner nom="Boubekeur BENZAID" titre="Front-End Developer"/>
  </div>
</template>

<script>
import Banner from './components/Banner.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'App',
  components: {
    Banner,
    Navbar
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Slab&display=swap');

*,::before,::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: 'Roboto Slab', serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
