<template>
    <div>
        <a :href="testimonial.link">
            <img :src="testimonial.img" :alt="testimonial.name">
            <h3>{{testimonial.name}}</h3>
            <p>{{testimonial.jobTitle}}</p>
        </a>
        <p class="testimonial">{{testimonial.testimonial}}</p>
    </div>
</template>

<script>
export default {
    name: "TestimonialCard",
    props: ["testimonial"]
}
</script>

<style scoped>
    div {
        max-width: 450px;
        margin: 2em auto;
        border-radius: 5px;
        background-color: #fff;
    }

    a {
        text-decoration: none;
        color: #1d3557;
    }

    img {
        border-radius: 50%;
        width: 100px;
        height: 100px;
        margin: 2em;
    }

    .testimonial {
        padding: 2em 3em;
    }
</style>