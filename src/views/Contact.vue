<template>
  <form name="contact" method="POST" data-netlify="true">
    <p>
      <label>Your Name: <input type="text" name="name" /></label>
    </p>
    <p>
      <label>Your Email: <input type="email" name="email" /></label>
    </p>

    <p>
      <label>Message: <textarea name="message"></textarea></label>
    </p>
    <p>
      <button v-on:click="handleSubmit" type="submit">Send</button>
    </p>
  </form>
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
