<template>
    <div>
        <p><span>👋</span> Hey there! Welcome to</p>
        <h1>Mike Parthum's Web Portfolio</h1>
    </div>
    
</template>

<script>
export default {
    name: "Greeting"
}
</script>

<style scoped>
    div {
        padding: 150px 0;
        background-image: linear-gradient(to bottom, rgba(168, 218, 220, 0.65), rgba(69, 123, 157, .7)),url('../../assets/coding.jpg');
        background-repeat: no-repeat;
        background-position: center right;
        background-size: cover;
        color: #fff;
    }

    span {
        font-size: 2em;
    }

    h1, p {
        text-shadow: 1px 0 4px #000;
    }

    p {
        font-weight: 600;
    }
</style>