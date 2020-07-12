<template>
    <div class="container">
        <div>
            <img src="@/assets/mikeparthum.png" alt="a picture of Mike Parthum">
            <p>Learn more on my LinkedIn page or my resume below!</p>
            <div class="icon-div">
                <a href="https://www.linkedin.com/in/michael-parthum/"><div class="icon linkedin"><i class="fab fa-linkedin"></i></div></a>
                <a href="@/assets/MikeParthumResume.pdf" download><div class="icon pdf"><i class="fas fa-file-pdf"></i></div></a>
                
            </div>
        </div>
        <div class="content">
            <H2 title="My Experience" />
            <p>I’ve loved technology since I was a child. When I was sixteen, I worked at CompUSA and 
                learned about computer components and more. I graduate from Franklin Pierce University 
                with BS in Finance in 2011.</p>
            <p>After starting my career in Fund Accounting, I began learning to automate Microsoft Excel 
                processes using Visual Basic for Applications (VBA). I was hooked. I started learning HTML, 
                CSS, JavaScript, Python and SQL. All on my own time and dime. Then I changed career paths 
                from Finance to Technology.</p>
        </div>
    </div>
</template>

<script>
import H2 from "@/components/partials/H2.vue"

export default {
    name: "Experience",
    components: {
        H2
    }
}
</script>

<style scoped>

    .container {
        max-width: 1000px;
        margin: auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        border-radius: 10px;
        background-color: #1d3557;
        color: #d3d3d3;
    }

    a {
        color: #d3d3d3;
    }

    img {
        margin: 2em auto;
        border: 3px solid #d3d3d3;
        border-radius: 50%;
    }

    p {
        padding: 0 2em;
    }

    .content p {
        margin: 2.5em;
    }

    .icon-div {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        font-size: 28px;
        margin: 2em auto;
    }

    .icon {
        border-radius: 50%;
        width: 50px;
        height: 50px;
        transition: ease-in all 0.1s;
        cursor: pointer;
    }

    .icon:hover {
        transform: translateY(-5px);
    }

    .icon i{
        position: relative;
        top: 6px;
    }

    .linkedin {
        background-color: #0077b5;
        
    }

    .pdf {
        background-color: #e63946;
    }

 
</style>