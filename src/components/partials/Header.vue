<template>
    <div class="nav-container">
        <nav>
            <div class="logo">
                <router-link to="/">
                    <img src="../../assets/logo.png" alt="logo">
                </router-link>
            </div>
            <div class="links">
                <router-link to="/projects">
                    <i class="fas fa-code"></i>
                </router-link>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped>
    .nav-container {
        background-color: #fff;
    }

    nav {
        display: flex;
        max-width: 750px;
        margin: 10px auto;
        justify-content: space-between;
        align-items: center;
    }
    .logo img{
        width: 65px;
        height: 65px;
        margin: 5px 15px;
    }

    .links {
        margin: auto 1em;
    }

    i{
        color: #1d3557;
        font-size: 1.8em;
     }
    
    i:hover {
        color: #e63946;
    }
</style>