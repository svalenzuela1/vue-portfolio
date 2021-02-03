<template>
    <div class="contact-sheet">
      <section>
        <form class="contact-form" name="form" method="POST" data-netlify="true">
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
              <b-button  label="Send message" type="submit" value="send" />
            </p>
          </b-field>
        </form>
      </section>
    </div>

</template>

<script>

export default{
  name: 'Contact',
}

</script>

<style>
.contact-sheet{
  padding-left: 10%;
  padding-right: 10%;
  padding-bottom: 10%;
}
</style>
