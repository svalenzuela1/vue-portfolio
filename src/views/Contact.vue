<template>
  <div class="contact-sheet">
  <section>
    <form class="contact-form" @submit.prevent="sendEmail">
    <b-field horizontal label="Subject" type="is-danger" message="Please enter a subject">
      <b-input name="subject" expanded></b-input>
    </b-field>

    <b-field horizontal label="From">
      <b-input name="name" placeholder="Name" expanded></b-input>
      <b-input name="email" type="email" placeholder="nobody@nowhere.com" expanded></b-input>
    </b-field>

    <b-field horizontal label="Message">
      <b-input type="textarea"></b-input>
    </b-field>

    <b-field horizontal><!-- Label left empty for spacing -->
      <p class="control">
        <b-button v-on:click="sendEmail" label="Send message" type="is-primary" value="send" />
      </p>
    </b-field>
    </form>
  </section>
  </div>
</template>

<script>
import emailjs from 'emailjs-com';

export default{
  name: 'Contact',
  data() {
    return {
      subject: '',
      name: '',
      email: '',
      message: ''
    }
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm('service_u1jml2x', 'template_hctlnqq', e.target,
            'user_OdKcH5LzTxMskLqSISB0r', {
              subject: this.subject,
              name: this.name,
              email: this.email,
              message: this.message
            })

      } catch(error) {
        console.log({error})
      }
      // Reset form field
      this.subject = ''
      this.name = ''
      this.email = ''
      this.message = ''
    },
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
