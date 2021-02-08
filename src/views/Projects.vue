<template>
  <b-carousel>
    <b-carousel-item v-for="(carousel, i) in carousels" :key="i">
      <section :class="`hero is-medium is-${carousel.color}`">
        <div class="hero-body has-text-centered">
          <h1 class="title">{{carousel.text}}</h1>
          <img :src="carousel.image">
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
        { image: 'https://res.cloudinary.com/stephaniev/image/upload/v1601580963/Screen_Shot_2020-10-01_at_3.34.58_PM_szxxol.png', text: 'Vooyage', color: 'primary' },
        { image: 'https://res.cloudinary.com/stephaniev/image/upload/v1601577889/Screen_Shot_2020-10-01_at_12.22.36_AM_onnyki.png', text: 'Quiz Customizer', color: 'info' },
        { image: 'https://res.cloudinary.com/stephaniev/image/upload/v1601581436/Screen_Shot_2020-10-01_at_3.43.22_PM_f8zusz.png', text: 'Savings Calculator', color: 'success' },
        { image: '', text: 'Fahrenheit vs. Celsius', color: 'warning' },
        //{ text: 'Slide 5', color: 'danger' }
      ]
    }
  }
}
</script>
