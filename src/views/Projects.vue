<template>
<div class="projects">
  <b-carousel>
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium is-${carousel.color}`">
        <div class="hero-body has-text-centered">
          <h1 class="title">{{carousel.text}}</h1>

          <a target="_blank" :href="carousel.API"><img class="links" src="../assets/icons8-api-48.png" v-if="carousel.API.length> 0"></a>
          <a target="_blank" :href="carousel.deployed"><img class="links" src="../assets/icons8-link-52.png"></a>
          <a target="_blank" :href="carousel.github"><img class="links" src="../assets/icons8-github-squared-64.png"></a><br>

          <img :src="carousel.image" class="carousel-image">

        </div>
      </section>
    </b-carousel-item>
  </b-carousel>
</div>
</template>

<script>
export default {
  name: 'Projects',
  data(){
    return {
      carousels: [
        { image: 'https://media.giphy.com/media/tH65wGj3847chND7Kl/giphy.gif', text: 'Vooyage', color: 'primary', github: 'https://github.com/e-mbrown/project3-frontend', deployed: 'https://vooyage.netlify.app/', API: 'https://github.com/e-mbrown/project3-backend'},
        { image: 'https://media.giphy.com/media/6C0MtSCcYM88XsQx3R/giphy.gif', text: 'Quiz Customizer', color: 'info', github: 'https://github.com/svalenzuela1/p4backend', deployed: 'https://quiz-customizer.netlify.app/', API: 'https://github.com/svalenzuela1/p4backend'},
        { image: 'https://media.giphy.com/media/jf1CiNrQfa8bGuvDJd/giphy.gif', text: 'Savings Calculator', color: 'success', github: 'https://github.com/svalenzuela1/savings-calculator', deployed: 'https://sale-savings-calc.netlify.app/', API: ''},
        { image: 'https://media.giphy.com/media/FmPfYzZzahN7HPivL4/giphy.gif', text: 'Fahrenheit vs. Celsius', color: 'warning', github: 'https://github.com/svalenzuela1/physics-calc', deployed: 'https://physics-calculator.herokuapp.com/', API: ''},
        //{ text: 'Slide 5', color: 'danger' }
      ]
    }
  }
}
</script>

<style>


.links{
  height: 8%;
  width: 8%;
  padding: 2%;
}


.carousel-image{
  width: 80%;
  height: 60%;
}

/*@media only screen and (max-width: 1024px) {*/
/*.links{*/
/*  height: 65px;*/
/*  width: 65px;*/
/*}*/

/*}*/

</style>
