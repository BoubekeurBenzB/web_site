<template>
  <div id="app">
    <Navbar></Navbar>
    <Banner nom="Boubekeur BENZAID" titre="Front-End Developer"/>
    <About
      title="I code, therefore I am."
      text="I am a young enthusiast who is keen on IT and anything about it since my first steps to High School. During the past few years, I gained lots of experience in this field due to the strong desire of becoming an expert. Today I am a senior front-end developer at one of the leading companies in the world."
      citation="“For me, web development is more than coding. It's a canvas with a blank page and I am the artist to paint it with colors of coding”."
      location="Based in Seattle"
    />
  </div>
</template>

<script>
import Banner from './components/Banner.vue'
import Navbar from './components/Navbar.vue'
import About from './components/About.vue'

export default {
  name: 'App',
  components: {
    Banner,
    Navbar,
    About
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
