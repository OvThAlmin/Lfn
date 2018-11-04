<template>
      <div class="column">
        <!-- Skills -->
        <div class="card">
          <div class="card-content skills-content">
            <h3 class="title is-4">Skills</h3>
            <div class="content">

              <article class="media" v-for="skill in skillSet.data" :key="skill.id">
                <div class="media-content">
                  <div class="content">
                    <p>
                      <strong>{{ skill.title }}</strong>
                      <br>
                      <progress class="progress is-primary" :value="skill.level" max="100"></progress>
                    </p>
                  </div>
                </div>
              </article>

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
            title: 'JavaScript:',
            level: 70
          },
          {
            title: 'Angular:',
            level: 55
          },
          {
            title: 'Nuxt.js:',
            level: 40
          },
          {
            title: 'Java/Spring:',
            level: 100
          },
          {
            title: 'Databases -MySQL',
            level: 95
          },
          {
            title: 'Databases -NoSQL',
            level: 80
          }
        ],
        name: ''
      }
    }
  }
}
</script>


<style>
.skills-content .media {
  margin: 0 !important;
  padding: 4px !important;
  border: 0 !important;
}

.skills-content .progress {
  height: 4px !important;
}
</style>

