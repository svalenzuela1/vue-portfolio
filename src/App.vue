<template>
  <div id="app" class="has-background-link-dark"> <!--NOTE: CHANGE COLOR LATER-->
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <Nav/>
    <Icons/>
    <router-view/>
  </div>
</template>
<script>
import Nav from './components/Nav.vue'
import Icons from './components/Icons.vue'
export default {
  name: 'App',
  components:{
    Nav, Icons
  }
}
</script>
<style>
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
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

Nav{
  padding: 50px;
}
</style>
