<template>
    <div class="container">
        <div>
            <img src="@/assets/mikeparthum.png" alt="a picture of Mike Parthum">
            <p>Learn more on my LinkedIn page or my resume below!</p>
            <div class="icon-div">
                <div class="icon linkedin"><i class="fab fa-linkedin"></i></div>
                <div class="icon pdf"><i class="fas fa-file-pdf"></i></div>
            </div>
        </div>
        <div class="content">
            <H2 title="My Experience" />
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
        justify-content: space-around;
        border: 2px solid #000;
    }

    .icon-div {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        font-size: 2em;
    }

    .icon {
        border-radius: 50%;
        height: 1.4em;
        width: 1.4em;
    }

    .linkedin {
        background-color: #0077b5;
    }

    .content {
        flex-grow: 2;
    }

</style>