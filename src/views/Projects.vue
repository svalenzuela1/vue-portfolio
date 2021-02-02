<template>
  <div class="about">


    <button v-on:click="fetchData">Get Data</button>
    <h1>{{ this.proj }}</h1>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  proj: '',
  url: 'https://spreadsheets.google.com/feeds/list/1UUsLTR3KfDVDztVxiJ9pC61R8jDDpiVVilF-fxHzp4U/od6/public/values?alt=json',
  fetchData: function(){
    fetch(this.url,{
      method: 'GET',
      headers: {
        'Content-Type': 'application/json'
      }
    })
    .then(response => response.json())
    .then(data => this.proj = data)
  },

}
</script>
