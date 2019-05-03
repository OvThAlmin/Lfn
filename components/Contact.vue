<template>
  <!-- Contact -->
  <section class="section" id="contact">
    <headline/>
    <!-- <contactForm/> -->
    <contactLink/>
  </section>
</template>

<script>
import Headline from "~/components/Contact/Headline.vue";
import ContactForm from "~/components/Contact/ContactForm.vue";
import ContactLink from "~/components/Contact/ContactLink.vue";

export default {
  components: {
    Headline,
    ContactForm,
    ContactLink
  }
};
</script>