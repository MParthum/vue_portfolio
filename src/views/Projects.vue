<template>
  <div class="about">
    <h1>Projects<span> by Mike Parthum</span></h1>
    <ProjectCardLarge v-bind:projects="projects" />
  </div>
</template>

<script>
import ProjectCardLarge from '@/components/ProjectCardLarge.vue'

export default {
  name: "Projects",
  components: {
    ProjectCardLarge
  },
  data () {
    return {
      projects: [
        {
          "title": "Web Development",
          "description": "Check out some of my web development work! My projects range from professional business sites to JavaScript games and some apps.",
          "img": require("@/assets/theluxedose.jpg")
        },
        {
          "title": "Power Platform",
          "description": "Microsoft's Platform, including Power Apps, Power BI, and Power Automate, is a great way to build business applications, fast.",
          "img": require("@/assets/FPADashboard.jpg")
        }
      ]
    }
  }
}
</script>

<style scoped>
  span {
    display: None;
  }
</style>
