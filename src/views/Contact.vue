<template>
  <div>
  <form name="form" netlify>
    <label v-for="(panelist, index) in panelists" :key="index">
      <input
          type="radio"
          name="panelist"
          @input="ev => form.askPerson = ev.target.value"
          :value="panelist"
          :checked="form.askPerson === panelist"
      />
      <span>{{ panelist }}</span>
    </label>
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
