<template>
    <div class="contact-sheet">
      <section>
        <form name="contact" netlify>
          <p>
            <label>Name <input type="text" name="name" /></label>
          </p>
          <p>
            <label>Email <input type="email" name="email" /></label>
          </p>
          <p>
            <button type="submit">Send</button>
          </p>
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
