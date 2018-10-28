<template>
    <div class="columns has-same-height is-gapless">
      <profile/>
      <pic/>
      <skill/>
    </div>
</template>

<script>
import Skill from '~/components/AboutMes/Skill/Skill.vue'
import Pic from '~/components/AboutMes/Skill/Pic.vue'
import Profile from '~/components/AboutMes/Skill/Profile.vue'

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

<style>
.has-same-height .card {
  height: 320px;
  overflow: hidden;
}
</style>

