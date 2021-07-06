<template>
  <div class="banner">
    <h1>{{ nom }}</h1>
    <h2>{{ titre }}</h2>
    <div class="links">
      <ul class="list">
        <li class="list-item">
          <a href="https://www.linkedin.com/in/boubekeur-benzaid/">
            <i class="fab fa-linkedin"></i>
          </a>
        </li>
        <li class="list-item">
          <a href="https://github.com/BoubekeurBenzB">
            <i class="fab fa-github-square"></i>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Banner',
  props: {
    nom: String,
    titre: String
  }
}
</script>

<style lang="scss" scoped>
.banner {
  // background-image: url(../assets/Banner.png);
  // background-repeat: no-repeat;
  // background-size: cover;
  background-color: #4d4d4d;
  background-position: center center;
  height: 90vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  position: relative;
}
h1 {
  color: #f1f1f1;
  font-size: 8em;
  max-width: 800px;
  text-align: center;
}
h2 {
  color: #d49e39;
  font-size: 4em;
}
.links {
  position: absolute;
  right: 10px;
  bottom: 10px;
  font-size: 2.5rem;
}
.list {
  list-style: none;
}
.list a {
  color: #f1f1f1;
  text-decoration: none;
}
</style>