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
        <p class="descrip">Software engineer who is interested in driving creative product development
          through software solutions that are accessible and transformative. While completing my degree
          in Communication Studies as a first generation college graduate, I discovered my passion for
          bridging the gap between people by utilizing logical frameworks. During my senior year of college
          I secured a full scholarship with the TechHire Open Code program in their partnership with General Assembly
          to pursue Software Development.</p>
      </fieldset>
<!--      </div>-->
    </div>

  <div class="skillsets">

    <fieldset class="fieldset2"><legend>SKILLS</legend>
<!--      <section> &lt;!&ndash; :class="`hero is-medium is-${carousel.color}`" &ndash;&gt;-->
        <div class="skillbox">
          <img class="skillchecks" src="../assets/icons8-html-48.png">
          <img class="skillchecks" src="../assets/icons8-css-48.png">
          <img class="skillchecks" src="../assets/icons8-javascript-50.png">
          <img class="skillchecks" src="../assets/icons8-vue-js-48.png">
          <img class="skillchecks" src="../assets/icons8-jquery-50.png">
          <img class="skillchecks" src="../assets/icons8-python-48.png">
          <img class="skillchecks" src="../assets/icons8-django-48.png">
          <img class="skillchecks" src="../assets/icons8-ruby-programming-language-50.png">
          <img class="skillchecks" src="../assets/rails-logo.png">
          <img class="skillchecks" src="../assets/icons8-command-line-48.png">
          <img class="skillchecks" src="../assets/icons8-heroku-50.png">
          <img class="skillchecks" src="../assets/icons8-git-squared-64.png">

        </div>
<!--      </section>-->
    </fieldset>
</div>

  </div>
</template>

<script>

export default {
  name: 'Home'}
</script>

<style>


.skillsets, .about
{
  padding: 5%;
}

.about, .name, .portfolioimg{
  padding: 1%;
  font-weight: bolder;
}
.home{
  padding-left: 20%;
  padding-right: 20%;
}

.name, p, legend{
  font-size: x-large;
  color: black;
  font-family: -apple-system;
}

.descrip{
  padding: 2%;
}

.portfolioimg{
  height: 50%;
  width: 50%;
}

.fieldset2{
  border: black solid 3px;
  font-family: -apple-system;
}

.fieldset2:nth-child(odd){
  font-weight: bolder;
}

.skillbox{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 5%;
}

.skillchecks{
  padding: 2%;
  height: 75px;
  width: 75px;
}

.skillchecks:hover{
  background-color: #42b983;
  animation: bounce 3s infinite;
}

@keyframes bounce {
  0%   { transform: scale(1,1)      translateY(0); }
  10%  { transform: scale(1.1,.9)   translateY(0); }
  30%  { transform: scale(.9,1.1)   translateY(-100px); }
  50%  { transform: scale(1.05,.95) translateY(0); }
  57%  { transform: scale(1,1)      translateY(-7px); }
  64%  { transform: scale(1,1)      translateY(0); }
  100% { transform: scale(1,1)      translateY(0); }
}

@media only screen and (min-width: 600px) and (max-width: 1022px) {

  .name, p, legend {
    font-size: large;
  }

}

@media only screen and (max-width: 599px) {

  .name, p, legend {
    font-size: medium;
  }

}

</style>
