<template>
  <div class="footer">

    <div class="div1">
    <h1>MADE WITH <img src="../assets/icons8-vue-js-48.png" class="footerimg"></h1>
    </div>

    <div class="div2">
    <H1>PORTFOLIO REPO <a target="_blank" href="https://github.com/svalenzuela1/vue-portfolio"><img class="footerimg" src="../assets/github.webp"></a></H1>
    </div>

  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style>
.footer{
  background-color: #3e3ea8!important;
}

.footerimg{
  height: 50px;
  width: 50px;
}

.div1, .div2{
  color: black!important;
}

@media only screen and (min-width: 1023px) {


.footer{
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-template-rows: repeat(6, 1fr);
  grid-column-gap: 0px;
  grid-row-gap: 0px;
}

.div1 { grid-area: 3 / 1 / 5 / 4; }
.div2 { grid-area: 3 / 4 / 5 / 7; }

.div1, .div2{
  color: black!important;
  font-size: x-large;
  font-family: -apple-system;
}

}
@media only screen and (max-width: 1022px) {
  .div1, .div2{
    display: flex;
    flex-direction: row;
    font-size: medium;
    justify-content: center;
  }

  .footerimg{
    height: 30px;
    width: 30px;
  }
}
</style>
