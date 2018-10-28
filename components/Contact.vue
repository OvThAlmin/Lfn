<template>
  <!-- Contact -->
  <section class="section" id="contact">
    <headline/>
    <contactForm/>
  </section>
</template>

<script>
import Headline from '~/components/Contact/Headline.vue'
import ContactForm from '~/components/Contact/ContactForm.vue'

export default {
  components: {
    Headline,
    ContactForm
  }
}
</script>