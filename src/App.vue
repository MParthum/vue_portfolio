<template>
  <div id="app">
    <Header />
    <router-view/>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/contact">Contact</router-link>
    </div>
    <p>Copyright &copy; {{currentYear}} Mike Parthum</p>
  </div>
</template>

<script>
import Header from './components/Header'
var currentYear = new Date().getFullYear()



export default {
  name: 'App',
  components: {
    Header
  },
  data() {
    return{
      currentYear
    }
  }
}
</script>

<style>

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
    background-color: #fcfafa;
    margin: -10px 0 0 0;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  #nav {
    padding: 30px;
  }

  #nav a {
    font-weight: bold;
    color: #1d3557;
    text-decoration: none;
  }

  #nav a:hover {
    color: #457b9d;
  }

  #nav a.router-link-exact-active {
    color: #e63946;
  }

  .btn {
    font-size: 1.2em;
    padding: 6px 25px;
    background: #e63946;
    border-radius: 15px;
    text-decoration: none;
    color: #fff;
    transition: .4s ease-out;
  }

  .btn:hover {
    background: #a8dadc;
    color: #1d3557;
  }

</style>
