<template >
  <div class="home">
<!--    <img alt="Vue logo" src="../assets/logo.png">-->
<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->


    <div class="about">
      <img class="portfolioimg" src="https://res.cloudinary.com/stephaniev/image/upload/v1602111407/IMG_2375_sv00u0.jpg" alt="image">

<!--      <div id="fieldset1">-->
        <h3 class="name">Hi, my name is </h3>
        <h1 class="name"> STEPHANIE VALENZUELA</h1>
      <fieldset class="fieldset2"> <legend> WHO AM I?</legend>
        <p id="fieldset1"> A Junior Developer who is driven to make an impact in the tech community.
          As a child of immigrants and a first generation College graduate, I joined
          TechHire Open Code four days after graduating college to pursue Software Development. I am passionate about
          logical thinking and problem-solving, constantly in pursuit of gaining more
          knowledge.</p>
      </fieldset>
<!--      </div>-->
    </div>

  <div class="skillsets">

    <fieldset class="fieldset2"><legend>Skills</legend>
<!--      <section> &lt;!&ndash; :class="`hero is-medium is-${carousel.color}`" &ndash;&gt;-->
        <div class="skillbox">
          <img src="../assets/icons8-html-50.png">
          <img src="../assets/icons8-css-50.png">
          <img src="../assets/icons8-javascript-50.png">
          <img src="../assets/icons8-vue-js-48.png">
          <img src="../assets/icons8-jquery-50.png">
          <img src="../assets/icons8-python-48.png">
          <img src="../assets/icons8-django-48.png">
          <img src="../assets/icons8-ruby-programming-language-50.png">


        </div>
<!--      </section>-->
    </fieldset>
</div>

  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  data(){
    return {
      skills: [
      "../assets/rails-logo.png",
          "../assets/icons8-python-48.png"
      ]
    }
  }
}
</script>

<style>


.skillsets, .about
{
  padding: 5%;
}

.about, .name, .portfolioimg{
  padding: 1%;
}
.home{
  padding-left: 20%;
  padding-right: 20%;
  padding-bottom: 10%;
}

.name, p, legend{
  font-size: x-large;
  color: black;
}

.portfolioimg{
  height: 50%;
  width: 50%;
}

.fieldset2{
  border: black solid 2px;
}

.skillbox{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
</style>
