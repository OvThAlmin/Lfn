<template>
    <!-- About -->
  <section class="section" id="skills">
    <div class="columns has-same-height is-gapless">
      <profile/>
      <pic/>
      
      <skill/>
    </div>
  </section>
</template>

<script>
import Skill from '~/components/Skill/Skill.vue'
import Pic from '~/components/Skill/Pic.vue'
import Profile from '~/components/Skill/Profile.vue'

export default {
  fetch({ store }) {
    store.commit('resetMenu')
  },
  components: {
    Skill,
    Pic,
    Profile
  }
}
</script>
