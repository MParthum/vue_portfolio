<template>
    <div class="container">
        <H2 title="Testimonials"/>
        <div class="testimonial">
            <div v-bind:key="testimonial.name" v-for="testimonial in testimonials">
                <TestimonialCard v-bind:testimonial="testimonial"/>
            </div>
        </div>
        
    </div>
</template>

<script>
import H2 from '@/components/partials/H2.vue'
import TestimonialCard from '@/components/partials/TestimonialCard'

export default {
    name: "Testimonials",
    components: {
        H2,
        TestimonialCard
    },
    props: ["testimonials"]
}
</script>

<style scoped>
    .container {
        max-width: 1000px;
        margin: auto;
    }
    .testimonial {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }
</style>