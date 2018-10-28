<template>
  <!-- Services -->
  <section class="section" id="services">
    <headline/>
    <serviceBox/>
  </section>
</template>

<script>
import Headline from '~/components/Services/ServiceHeadline.vue'
import ServiceBox from '~/components/Services/ServiceBox.vue'

export default {
  components: {
    Headline,
    ServiceBox
  }
}
</script>