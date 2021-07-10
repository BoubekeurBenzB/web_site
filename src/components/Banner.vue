<template>
  <section class="banner">
    <div class="overlay"></div>
    <div class="content">
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
  </section>
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
  background-image: url(../assets/Banner.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #4d4d4d;
  background-position: center center;
  height: 70vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  position: relative;
}
.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  z-index: 1;
  background-color: #17151a;
  opacity: 0.6;
}
.content {
  text-align: center;
  z-index: 2;
}
h1 {
  color: #f1f1f1;
  font-size: clamp(40px, 8vw, 80px);
}
h2 {
  color: #d49e39;
  font-size: clamp(30px, 5vw, 60px);
}
.links {
  position: absolute;
  right: 1rem;
  bottom: 1rem;
  font-size: clamp(30px, 5vw, 40px);
}
.list {
  list-style: none;
}
.list a {
  color: #f1f1f1;
  text-decoration: none;
}

/** responsive */

/** tablet & ipad */
@media screen and (max-width: 1024px) {
  .links {
    top: 80%;
    bottom: 0;
    left: 50%;
    right: 0;
    transform: translate(-50%, -50%);
  }
  .list-item {
    display: inline-block;
    margin-left: 1rem;
  }
}
</style>