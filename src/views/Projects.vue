<template>
  <b-carousel>
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium is-${carousel.color}`">
        <div class="hero-body has-text-centered">
          <h1 class="title">{{carousel.text}}</h1>
        </div>
      </section>
    </b-carousel-item>
  </b-carousel>
</template>

<script>
export default {
  name: 'Projects',
  data(){
    return {
      carousels: [
        { image: '', text: 'Vooyage', color: 'primary' },
        { image: '', text: 'Quiz Customizer', color: 'info' },
        { image: '', text: 'Savings Calculator', color: 'success' },
        { image: '', text: 'Fahrenheit vs. Celsius', color: 'warning' },
        //{ text: 'Slide 5', color: 'danger' }
      ]
    }
  }
}
</script>
