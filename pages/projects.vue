<template>
  <main>
      <h1>Projects</h1>
      <div v-for="project in githubProjects" :key="project.id">
        <h3><a :href="project.html_url">{{ project.name }}</a></h3>
      </div>
  </main>
</template>

<script>
import { mapState } from 'vuex'

export default {
  computed: {
    ...mapState(["githubProjects"])
  },
  mounted() {
    this.$store.dispatch("getGithubProjects");
  }
}
</script>

<style scoped>
main {
  width: 80vw;
  margin: 2% 8%;
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: 1fr;
  grid-column-gap: 50px;
  grid-row-gap: 0px;

}
aside {
  grid-area: 1 / 2 / 2 / 3;
}
section {
  grid-area: 1 / 1 / 2 / 2;
  background: white;
  color: black;
  padding: 30px;
}
  a {
  color: black;
}
.stars {
  color: orangered;
}
.project {
  margin-bottom: 30px;
}
</style>
