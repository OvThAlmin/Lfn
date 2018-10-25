<template>
<div>
  <section class="hero is-primary is-bold">
    <div class="hero-body">
      <h1 class="title is-size-2">
        About
      </h1>
      <h2 class="subtitle is-size-4">
        ねこ
      </h2>
    </div>
  </section>
  
  <aboutme/>
  <skills/>
</div>
</template>

<script>
import Aboutme from '~/components/Aboutme.vue'
import Skills from '~/components/Skills.vue'

export default {
  fetch({ store }) {
    store.commit('resetMenu')
  },
  components: {
    Aboutme,
    Skills
  }
}
</script>