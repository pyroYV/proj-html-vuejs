<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header/Header.vue';
import Main from './components/Main/Main.vue';
import Footer from './components/Footer/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer

  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css");
a{
    color: white;
    text-decoration: none;
    &:hover{
      color: whitesmoke;
    }
}

ul{
  list-style: none;
  li{
    display: inline;
  }
}

@font-face {
  font-family: "AbrilFatface";
  font-display: auto;
  src: local('AbrilFatface'); 
  url:("./fonts/AbrilFatface-Regular.ttf");
}
</style>
