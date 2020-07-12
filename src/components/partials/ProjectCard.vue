<template>
    <div class="container">
       <img :src="project.img" alt="broken">
       <h3>{{project.title}}</h3>
       <p>{{project.description}}</p>
       <router-link to="/about" class="btn">Learn More</router-link>
    </div>
</template>

<script>
export default {
    name: "ProjectCard",
    props: ["project"]
}
</script>

<style scoped>
    img {
        max-width: 320px;
        margin: 2em auto;
        }
    
    p {
        margin: 2.5em;
    }
</style>