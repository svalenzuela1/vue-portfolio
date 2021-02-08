<template>
<div class="projects">
  <b-carousel>
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium is-${carousel.color}`">
        <div class="hero-body has-text-centered">
          <h1 class="title">{{carousel.text}}</h1>
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
        { image: 'https://media.giphy.com/media/tH65wGj3847chND7Kl/giphy.gif', text: 'Vooyage', color: 'primary', github: 'https://github.com/e-mbrown/project3-frontend', deployed: 'https://vooyage.netlify.app/'},
        { image: 'https://media.giphy.com/media/6C0MtSCcYM88XsQx3R/giphy.gif', text: 'Quiz Customizer', color: 'info', github: 'https://github.com/svalenzuela1/p4backend', deployed: 'https://quiz-customizer.netlify.app/'},
        { image: 'https://media.giphy.com/media/jf1CiNrQfa8bGuvDJd/giphy.gif', text: 'Savings Calculator', color: 'success', github: 'https://github.com/svalenzuela1/savings-calculator', deployed: 'https://sale-savings-calc.netlify.app/'},
        { image: '', text: 'Fahrenheit vs. Celsius', color: 'warning' },
        //{ text: 'Slide 5', color: 'danger' }
      ]
    }
  }
}
</script>

<style>


.links{
  height: 100px;
  width: 100px;
  padding: 2%;
}



.carousel-image{
  width: 80%;
  height: 60%;
}
</style>
