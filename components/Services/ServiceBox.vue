<template>
   <!-- Services -->
    <div class="container">
      <div class="columns">
       <div class="column"  v-for="skill in skillSet.data" :key="skill.id">
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
      database: 'demo',
      skillSet: {
        data: [
          {
            title: 'Infrastructure',
            detail:
              'Migrate Cassandra to MySQL by Aurora. Develop This page by Netlify.'
          },
          {
            title: 'Back End Web Development',
            detail:
              'Develop Back End application/service using Spring Framework by Java 8.'
          },
          {
            title: 'Database',
            detail:
              'Develop and Design MySQL by Amazon Aurora and Cassandra databases.'
          },
          {
            title: 'Front End Web Development',
            detail:
              'Develop Front End using latest standards with HTML5/CSS3 with added funtionality using JavaScript and Vue.js.'
          }
        ],
        name: ''
      }
    }
  }
}
</script>
