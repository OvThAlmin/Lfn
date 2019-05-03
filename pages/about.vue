<template>
  <div>
    <section class="hero is-primary is-bold">
      <div class="hero-body">
        <h1 class="title is-size-2">About</h1>
        <h2 class="subtitle is-size-4">ねこ</h2>
      </div>
    </section>

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
  fetch({ store }) {
    store.commit("resetMenu");
  },
  components: {
    Aboutme,
    Services,
    Contact
  }
};
</script>