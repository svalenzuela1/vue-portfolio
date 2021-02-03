<template>
  <div class="contact-sheet">
  <section>
    <form action="https://docs.google.com/forms/d/e/1FAIpQLSciTpkSCmvIMNliYziyj1vPooUO7Ixjk3IE0PBJ67_EgErdMg/viewform" method="post">
      <label>Name*</label>
      <input type="text" placeholder="Name*" name="Name" required>

      <label>Email Address*</label>
      <input type="email" placeholder="Email address*" name="Email" required>

      <label>Subject</label>
      <input type="text" placeholder="Subject" name="Subject" required>

      <label>Message*</label>
      <textarea rows="5" placeholder="Message*" name="Message" required></textarea>

      <button type="submit">Send</button>
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
