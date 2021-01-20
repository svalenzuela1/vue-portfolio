<template >
  <div class="home">
<!--    <img alt="Vue logo" src="../assets/logo.png">-->
<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->



      <img class="portfolioimg" src="https://res.cloudinary.com/stephaniev/image/upload/v1602111407/IMG_2375_sv00u0.jpg" alt="image">

<!--      <div id="fieldset1">-->
        <h3 class="name">Hi, my name is </h3>
        <h1 class="name"> STEPHANIE VALENZUELA</h1>
      <fieldset class="name"> <legend> WHO AM I?</legend>
        <p id="fieldset1"> A Junior Developer who is driven to make an impact in the tech community.
          As a child of immigrants and a first generation College graduate, I joined
          TechHire Open Code four days after graduating college to pursue Software Development. I am passionate about
          logical thinking and problem-solving, constantly in pursuit of gaining more
          knowledge.</p>
      </fieldset>
<!--      </div>-->
    </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {

  }
}
</script>

<style>
.home{
  padding: 30px;
}

.name{
  font-size: x-large;
}

#fieldset1{
  padding-left: 300px;
  padding-right: 300px;
}

.portfolioimg{
  height: 30%;
  width: 30%;
}
</style>
