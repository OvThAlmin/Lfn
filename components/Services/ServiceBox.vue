<template>
  <!-- Services -->
  <div class="container">
    <div class="columns">
      <div class="column" v-for="skill in skillSet.data" :key="skill.id">
        <div class="box">
          <div class="content">
            <h4 class="title is-5">{{ skill.title }}</h4>
            {{ skill.detail }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      database: "demo",
      skillSet: {
        data: [
          {
            title: "Front End Web Development",
            detail:
              "Develop Front End using TypeScript with added funtionality using Angular and Nuxt.js."
          },
          {
            title: "Back End Web Development",
            detail:
              "Develop Back End application/service using Spring Framework by Java 8."
          },
          {
            title: "Database",
            detail:
              "Develop and Design MySQL in Amazon Aurora and Cassandra databases."
          },
          {
            title: "Infrastructure",
            detail: "Build and Deploy This page by Netlify."
          }
        ],
        name: ""
      }
    };
  }
};
</script>
