<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <a target="_blank" href="https://github.com/svalenzuela1">
      <img class="logo" src="https://cdn3.iconfinder.com/data/icons/inficons/512/github.png">
    </a>
    <a target="_blank" href="https://www.linkedin.com/in/stephanie-val/">
      <img class="logo" src="https://cdn.iconscout.com/icon/free/png-256/linkedin-2662666-2213265.png">
    </a>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
