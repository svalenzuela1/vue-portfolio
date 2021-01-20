<template class="nav">
  <b-navbar class="has-background-link-dark"> <!--class gives it color: NOTE CHANGE COLOR LATER-->
    <template #brand class="try">
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
<!--        <img-->
<!--            src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"-->
<!--            alt="Lightweight UI components for Vue.js based on Bulma"-->
<!--        >-->
      </b-navbar-item>
    </template>
    <template #start>
      <router-link to="/">
      <b-navbar-item href="#" class="navbar-item">
        Home
      </b-navbar-item>
    </router-link>
      <router-link to="/projects">
      <b-navbar-item href="#">
        Projects
      </b-navbar-item>
      </router-link>

        <b-navbar-item href="#">
          Contact Me
        </b-navbar-item>

    </template>

    <template #end>
      <b-navbar-item tag="div">
        <div class="buttons">

          <a class="resume-link" type="is-primary is-light" href="https://drive.google.com/file/d/1TAj2-vJIDwMgDhTHkAuQrWNHPoCg812z/view">
            Resume
          </a>
        </div>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>




    <script>
      export default{
        name: "Nav",
      }
    </script>

<style>
.navbar-item{
  font-size: x-large;
  color: white;
}
.resume-link{
  font-size: x-large;
}
.try{
color: navy;
}

.nav{
  padding: 20px;
}
</style>
