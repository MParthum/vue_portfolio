<template>
  <div class="home">
    <Greeting />
    <Work v-bind:projects="projects"/>
    <Experience />
    <Testimonials v-bind:testimonials="testimonials"/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Greeting from '@/components/partials/Greeting.vue'
import Work from '@/components/partials/Work.vue'
import Experience from '@/components/partials/Experience.vue'
import Testimonials from '@/components/partials/Testimonials.vue'
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    Greeting,
    Work,
    Experience,
    Testimonials
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
      ],
      testimonials : [
        {
          "name": "Rob Lemieux",
          "jobTitle": "Fund Reporting Analyst",
          "img": require("@/assets/rob.jpg"),
          "link": "https://www.linkedin.com/in/rob-lemieux-ba01a212/",
          "testimonial": "I had the absolute pleasure of working with Mike during our time at Fidelity. In all my years at Fidelity, I don't believe I have worked with anyone that could match Mike's penchant for improving every process he touched. His dedication to and passion for technology as a solution to hurdles we face every day has proven to be a boon in my own career as it taught me how to think like a systems analyst. His knack for design should not go unmentioned because he has a true eye for intuitive and easy design. You could always tell an application/macro that was designed by Mike. I have told Mike this before, but it bears repeating: if I were starting a company tomorrow, he'd be my first call for a partner."
        },
        {
          "name": "Matt Donovan",
          "jobTitle": "Senior Data Solutions Analyst",
          "img": require("@/assets/matt.jpg"),
          "link": "https://www.linkedin.com/in/mattjamesdonovan/",
          "testimonial": "I’ve had the pleasure of managing Michael in one role and working with him as a peer and mentor in a newer role I had taken on and his skills and aptitude to learn new things and tackle all challenges has spanned across our entire professional relationship. When he was my direct report, it was easy to give him requirements and trust he would deliver results. He demonstrated Agile methods before Agile became the trend and that goes to show how Mike is always thinking forward. As a peer and mentor in my current role, I have been able to count on him as a resource in a new working environment and, as always, a technical resource who always wants to help solve a problem. On top of being a great worker, he is a terrific teammate with whom everyone, including myself, has always enjoyed working."
        }
      ]
    }
  }
}
</script>
