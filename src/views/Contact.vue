<template>
  <div>
  <form name="form" netlify>
<input name="name" placeholder="name">
  </form>
    <button v-on:click="handleSubmit">Submit</button>
  </div>
</template>
<script>
import axios from 'axios'
export default {
  name: "QAForm",
  data () {
    return {
      form: {
        askPerson: ''
      }
    }
  },
  methods: {
    handleSubmit () {
      axios.post('/', {

      })
          .then(() => {
            this.$router.push('thanks')
          })
          .catch(() => {
            this.$router.push('404')
          })
    }
  }
}
</script>

<style>
.contact-sheet{
  padding-left: 10%;
  padding-right: 10%;
  padding-bottom: 10%;
}
</style>
