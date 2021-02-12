<template>
  <div id="app" :style="myStyle"> <!--NOTE: CHANGE COLOR LATER-->
    <Nav :style="myStyle"/>
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
  },
  data: function(){
    return {
      myStyle:{
        backgroundColor: "#3e3ea8",
        // color: "f5f5f7"
      }
    }
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

/*#nav a {*/
/*  font-weight: bold;*/
/*  color: #2c3e50;*/
/*}*/

/*#nav a.router-link-exact-active {*/
/*  color: #42b983;*/
/*}*/

Nav{
  padding: 50px;
  color: #2c3e50;
  font-weight: bold;
}

</style>
