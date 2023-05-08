<template>
<Navbar></Navbar>
<router-view></router-view>
<Footer></Footer>
</template>

<style>
#app {
  font-family:'Raleway', sans-serif;;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #80836C;
  color: #ffffff;
  min-height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';
export default {
  components : {
    Navbar,
    Footer
  }
}
</script>
