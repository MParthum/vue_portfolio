<template>
  <div class="home">
    <Greeting />
    <Work v-bind:projects="projects"/>
    <Experience />
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Greeting from '@/components/partials/Greeting.vue'
import Work from '@/components/partials/Work.vue'
import Experience from '@/components/partials/Experience.vue'
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Greeting,
    Work,
    Experience
  },
  data() {
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
