<template>
    <div class="container">
        <h3>{{project.title}}</h3>
       <img :src="project.img" alt="broken">
       <p>{{project.description}}</p>
       <div class="project-btns">
            <a v-if="project.link != ''" :href="project.link" class="btn">Check It Out</a>
            <a v-if="project.github != ''" :href="project.github" class=" btn github-btn">View on Github</a>
       </div>
       
    </div>
</template>

<script>
export default {
    name: "ProjectCardLarge",
    props: ["project"]
}
</script>

<style scoped>
    .container {
        background-color: #fff;
        border-radius: 5px;
        padding: 2em;
    }

    h3 {
        text-transform: uppercase;
    }

    img {
        max-width: 550px;
        margin: 2em auto;
        border-radius: 5px;
        width: 100%;
    }
    
    p {
        margin: 2.5em;
    }

    .project-btns{
        display: flex;
        justify-content: space-evenly;
    }
</style>