<template>
    <div class="container">
        <H2 title="My Work" />
        <div class="project-container">
          <div v-bind:key="project.title" v-for="project in projects" class="project">
            <ProjectCard v-bind:project="project"/>
          </div>
        </div>
    </div>
</template>

<script>
import ProjectCard from "./ProjectCard"
import H2 from "../partials/H2"

export default {
  name: "Work",
  components: {
      ProjectCard,
      H2
    },
  props: ["projects"]
}
</script>

<style scoped>
  
  .project-container {
    max-width: 1000px;
    margin: 2em auto;
    display: flex;
    flex-wrap: wrap;
    justify-content:space-around;
    align-content: center;

  }
  .project {
    max-width: 375px;
    padding-bottom: 2em;
  }

</style>