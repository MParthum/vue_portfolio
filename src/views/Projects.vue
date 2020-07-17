<template>
  <div class="container">
    <h1>Projects<span> by Mike Parthum</span></h1>
    <div class="line"></div>
    <div class="project-container">
      <div v-bind:key="project.title" v-for="project in projects" class="project">
        <ProjectCardLarge v-bind:project="project"/>
      </div>
    </div>
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
          "title": "The Luxe Dose",
          "type": "Web Development",
          "link": "https://theluxedose.com/",
          "github": "https://github.com/MParthum/luxedose",
          "description": "The Luxe Dose is a medical spa based in Belmont, MA. This entire website was created from a blank screen – using only HTML, CSS/Sass, and JavaScript. I’m particularly pleased with how the ‘Learn More’ content is handled on this page. When a user clicks on a ‘Learn More’ button, the content expands and scrolls the screen accordingly. If the user does not want to read about other services, they can simply continue scrolling and the page flow is still intact. Check it out here: ",
          "img": require("@/assets/theluxedose.jpg")
        },
        {
          "title": "Financial Inquiries Service Desk",
          "type": "Power Platform",
          "link": "",
          "github": "",
          "description": "I created a customized, branded service desk for my employer to capture all data points required for financial inquiries throughout the organization. I used Microsoft’s Power Platform in addition to SharePoint to complete this project. The business stakeholders specifically did not want to use JIRA. For ease of access to perform CRUD operations (Create, Read, Update, and Delete), SharePoint was used since this service desk will live in a Microsoft Teams channel. When access to the Teams channel is granted, so is access to the underlying SharePoint site. Microsoft Power Apps is how the application was built. Power Automate was leveraged to send out email notifications (with Deep Links for ease of use). Power BI is used for managers to track the service desk tickets. If I were to make changes to this application, I would have used a database rather than SharePoint. SharePoint has delegation limitations as soon as Lists contain more than 500 records. There is an option to increase the limit to 2,000 (which I did); however, this still requires maintenance of the SharePoint List to keep all functionality working properly. ",
          "img": require("@/assets/FPADashboard.jpg")
        },
        {
          "title": "Ba Dum Tssss",
          "type": "Web Development",
          "link": "https://mparthum.github.io/drumkit/",
          "github": "https://github.com/MParthum/drumkit",
          "description": "I love music. I play guitar and bass for fun since my dream of being a musician didn’t work out. 😐 Every once in a while I get the urge to play the drums, so why not play them for free?!?! This project is done with HTML, CSS, and JavaScript. This was one of my first web projects after learning JavaScript and the assets were provided through a Udemy course I completed. This project during the class did not provide the solution at the end. The Q&A section had numerous people asking for help. I solved the issues on my own and was eager to jump in and help others. Check out the project here and relieve some stress in the process: https://mparthum.github.io/drumkit/ Check out the repository here: https://github.com/MParthum/drumkit ",
          "img": require("@/assets/drumkit.jpg")
        },
        {
          "title": "My Portfolio",
          "type": "Web Development",
          "link": "https://mikeparthum.com/",
          "github": "https://github.com/MParthum/vue_portfolio",
          "description": "I created a customized, branded service desk for my employer to capture all data points required for financial inquiries throughout the organization. I used Microsoft’s Power Platform in addition to SharePoint to complete this project. The business stakeholders specifically did not want to use JIRA. For ease of access to perform CRUD operations (Create, Read, Update, and Delete), SharePoint was used since this service desk will live in a Microsoft Teams channel. When access to the Teams channel is granted, so is access to the underlying SharePoint site. Microsoft Power Apps is how the application was built. Power Automate was leveraged to send out email notifications (with Deep Links for ease of use). Power BI is used for managers to track the service desk tickets. If I were to make changes to this application, I would have used a database rather than SharePoint. SharePoint has delegation limitations as soon as Lists contain more than 500 records. There is an option to increase the limit to 2,000 (which I did); however, this still requires maintenance of the SharePoint List to keep all functionality working properly. ",
          "img": require("@/assets/portfolio.jpg")
        }
      ]
    }
  }
}
</script>

<style scoped>
  .container {
    max-width: 1000px;
    margin: auto;
  }

  span {
    display: None;
  }

  .project {
    margin: 2em;
  }

  h1 {
    margin: 1.5em auto 0;
    text-transform: uppercase;
  }

  .line {
    height: 4px;
    width: 75px;
    background-color: #e63946;
    margin: 0 auto;
  }

</style>
