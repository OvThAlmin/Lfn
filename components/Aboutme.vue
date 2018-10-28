<template>
    <!-- About -->
    <section class="section" id="about">
      <!-- Title -->
      <introduction/>
      <skills/>
  </section>
</template>

<script>
import Skills from '~/components/AboutMes/Skills.vue'
import Introduction from '~/components/AboutMes/Introduction.vue'

export default {
  fetch({ store }) {
    store.commit('resetMenu')
  },
  components: {
    Skills,
    Introduction
  }
}
</script>