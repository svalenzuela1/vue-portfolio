<template>
  <div class="container">
      <form class="contact-form" @submit.prevent="sendEmail">
        <label>Name</label>
        <input type="text" name="user_name">
        <label>Email</label>
        <input type="email" name="user_email">
        <label>Message</label>
        <textarea name="message"></textarea>
        <input type="submit" value="Send">
      </form>
  </div>
    </template>

<script>
import emailjs from 'emailjs-com';

export default {
  name: 'Contact',
  methods: {
    sendEmail: (e) => {
      emailjs.sendForm('service_u1jml2x', 'template_hctlnqq', e.target, 'user_OdKcH5LzTxMskLqSISB0r')
          .then((result) => {
            console.log('SUCCESS!', result.status, result.text);
          }, (error) => {
            console.log('FAILED...', error);
          });
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

<style>
.contact-sheet{
  padding-left: 10%;
  padding-right: 10%;
  padding-bottom: 10%;
}

* {box-sizing: border-box;}

.container {
  display: block;
  margin:auto;
  text-align: center;
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
  width: 50%;
}

label {
  float: left;
}

input[type=text], [type=email], textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}

input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
}
</style>
