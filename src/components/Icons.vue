<template>
  <div class="icons">

    <a target="_blank" href="https://github.com/svalenzuela1">
      <img class="logo" src="../assets/github.webp">
    </a>


    <a target="_blank" href="https://www.linkedin.com/in/stephanie-val/">
      <img class="logo" src="https://cdn.iconscout.com/icon/free/png-256/linkedin-2662666-2213265.png">
    </a>
  </div>
</template>

<script>
export default {
  name: 'Icons',
}
</script>
<style>
@media only screen and (min-width: 1024px) {

.logo{
  height: 60px;
  width: 60px;
}

.icons{
  display: flex;
  flex-direction: column;
  padding: 50px;
  position: fixed;
}

.icons::after{
  content: "";
  display: block;
  width: 1px;
  height: 100px;
  margin: 0px auto;
  background-color: black;
}
}
@media only screen and (max-width: 1023px) {
  .icons{
    display: none;
  }
}
</style>
