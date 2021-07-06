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
*,::before,::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
