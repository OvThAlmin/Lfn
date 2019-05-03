<template>
  <div>
    <aboutme/>
    <services/>
    <contact/>
  </div>
</template>

<script>
import Aboutme from "~/components/Aboutme.vue";
import Services from "~/components/Services.vue";
import Contact from "~/components/Contact.vue";
export default {
  components: {
    Aboutme,
    Services,
    Contact
  },
  fetch({ store }) {
    store.commit("resetMenu");
  }
};
</script>
