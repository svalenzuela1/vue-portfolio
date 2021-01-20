<template>
  <div class="icons">

    <a target="_blank" href="https://github.com/svalenzuela1">
      <img class="logo" src="https://cdn3.iconfinder.com/data/icons/inficons/512/github.png">
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

</style>
