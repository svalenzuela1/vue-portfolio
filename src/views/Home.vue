<template >
  <div class="home">
<!--    <img alt="Vue logo" src="../assets/logo.png">-->
<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <div class="icons">

    <a target="_blank" href="https://github.com/svalenzuela1">
      <img class="logo" src="https://cdn3.iconfinder.com/data/icons/inficons/512/github.png">
    </a>


    <a target="_blank" href="https://www.linkedin.com/in/stephanie-val/">
      <img class="logo" src="https://cdn.iconscout.com/icon/free/png-256/linkedin-2662666-2213265.png">
    </a>
    </div>
    <div class="about">

      <img class="portfolioimg" src="https://res.cloudinary.com/stephaniev/image/upload/v1602111407/IMG_2375_sv00u0.jpg" alt="image">

      <div id="fieldset1">
        <h3 id="aboutMe">Hi, my name is </h3>
        <h1 class="name"> STEPHANIE VALENZUELA</h1>
      <fieldset class="fieldset1"> <legend> WHO AM I?</legend>
        <p> A Junior Developer who is driven to make an impact in the tech community.
          As a child of immigrants and a first generation College graduate, I joined
          TechHire Open Code four days after graduating college to pursue Software Development. I am passionate about
          logical thinking and problem-solving, constantly in pursuit of gaining more
          knowledge.</p>
      </fieldset>
      </div>
    </div>
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
template{
  background-color: navy;
}
.logo{
  height: 100px;
  width: 100px;
  background-color: white;
}

.icons{
  display: flex;
  flex-direction: column;
 align-items: flex-start;
  padding: 20px;
  position: fixed;
}

.icons::after{
  content: "";
  display: block;
  width: 1px;
  height: 90px;
  margin: 0px auto;
  background-color: black;
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
