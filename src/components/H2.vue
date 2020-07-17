<template>
    <div>
        <h2>{{title}}</h2>
        <div class="line"></div>
    </div>
</template>

<script>
export default {
    name: "Experience",
    props: ["title"]
}
</script>

<style scoped>
    h2 {
    margin-top: 2.5em;
    text-transform: uppercase;
  }

  .line {
    height: 4px;
    width: 75px;
    background-color: #e63946;
    margin: 0 auto;
  }
</style>