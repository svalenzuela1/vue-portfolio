<template class="nav">

  <b-navbar> <!--class gives it color: NOTE CHANGE COLOR LATER-->

    <template #brand>
      <b-navbar-item tag="router-link" :to="{ path: '/' }">
<!--        <img-->
<!--            src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"-->
<!--            alt="Lightweight UI components for Vue.js based on Bulma"-->
<!--        >-->
<!--      <p>Made With</p> <img src="../assets/logo.png">-->
      </b-navbar-item>
    </template>
    <template #end>

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

      <router-link to="/contact">
        <b-navbar-item href="#">
          Contact Me
        </b-navbar-item>
      </router-link>

      <b-navbar-item href="#">
      <a target="_blank" class="resume-link" type="is-dark" href="https://drive.google.com/file/d/1j9TtTRf6_Lxn7vdExCoWwUmqwPs3_-C1/view?usp=sharing">
        Resume
      </a>
      </b-navbar-item>

    </template>

<!--    <template #end>-->
      <b-navbar-item tag="div">
<!--        <div class="buttons">-->

<!--          <a target="_blank" class="resume-link" type="is-primary is-light" href="https://drive.google.com/file/d/1TAj2-vJIDwMgDhTHkAuQrWNHPoCg812z/view">-->
<!--            Resume-->
<!--          </a>-->
<!--        </div>-->
      </b-navbar-item>
<!--    </template>-->

  </b-navbar>

</template>

    <script>
      export default{
        name: "Nav",
        data: function() {
          return {
            style: {
              backgroundColor: "#344189",
              color: "#efefee",
              fontSize: 30
            },
          }
        },
      }
    </script>

<style>

.resume-link {
  color: black!important;
}

@media only screen and (min-width: 1024px) {

  .navbar-item{
    font-size: x-large;
    color: black!important;
  }

  .nav {
    padding: 10%;
  }


}
@media only screen and (max-width: 1022px) {
  .nav{
    padding: 20px;
  }

  /*.navbar-item{*/
  /*  border: black solid 2px;*/
  /*}*/
  .navbar-burger.burger:hover{
    background-color: white;
    color: black!important;
  }

  span{
    color: black;
  }
}
</style>
