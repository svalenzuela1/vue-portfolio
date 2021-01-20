<template>
  <div class="icons">

    <a target="_blank" href="https://github.com/svalenzuela1">
      <img class="logo" src="https://cdn3.iconfinder.com/data/icons/free-social-icons/67/github_circle_black-512.png">
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
.logo{
  height: 100px;
  width: 100px;
}

.icons{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 50px;
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

</style>
