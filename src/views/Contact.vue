<template>

  <div class="contact-sheet">
    <section>
      <form class="contact-form" @submit.prevent="sendEmail">
    <b-field horizontal label="Subject" type="is-danger" message="Please enter a subject">
      <b-input v-model="subject" name="subject" expanded></b-input>
    </b-field>

    <b-field horizontal label="From">
      <b-input v-model="name" name="user_name" placeholder="Name" expanded></b-input>
      <b-input v-model="email" name="user_email" type="email" placeholder="nobody@nowhere.com" expanded></b-input>
    </b-field>

    <b-field horizontal label="Message">
      <b-input v-model="message" type="textarea" name="message"></b-input>
    </b-field>

    <b-field horizontal><!-- Label left empty for spacing -->
      <p class="control">
        <input type="submit" value="Send" v-on:click="sendEmail">
      </p>
    </b-field>
        </form>
    </section>
  </div>

    </template>

<script>
import emailjs from 'emailjs-com';

export default {
  name: 'Contact',
  data: function(){
    return{
      subject: "",
      name: "",
      email: "",
      message: ""

    }
  },
  methods: {
    redirect: function(){
      return this.$router.push("/thanks")
    },
    sendEmail: (e) => {
      emailjs.sendForm('service_u1jml2x', 'template_hctlnqq', e.target, 'user_OdKcH5LzTxMskLqSISB0r')
      alert('Thank you for your email! I will get back to you as soon as possible.')
      e.target.reset() //will reset the form
      this.redirect() //an attempt to display thank you page

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


