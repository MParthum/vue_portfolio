<template>
    <div class="container">
        <H2 title="Say Hello" />
        <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSea-pKLYm5z9L_2zZElYeLlencLZL77SlukPwQ208KWlxQtZg/viewform?embedded=true" 
            class="my-frame" width="650" height="850" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
    </div>
</template>

<script>
import H2 from '@/components/partials/H2.vue'

export default {
    name: "Contact",
    components: {
        H2
    }
}
</script>

<style scoped>
    .container {
        max-width: 1000px;
        margin: auto;
    }

    .my-frame {
        width: 100%;
        margin: 2em auto;
    }
</style>