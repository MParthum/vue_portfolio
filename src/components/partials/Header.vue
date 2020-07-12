<template>
    <div class="nav-container">
        <nav>
            <div class="logo">
                <router-link to="/">
                    <img src="../../assets/logo.png" alt="logo">
                </router-link>
            </div>
            <div class="links">
                <ul>
                    <li>
                        <router-link to="/about">
                            <i class="fas fa-code"></i>
                        </router-link>
                    </li>
                    <li>
                        <router-link to="/about">
                            <i class="fas fa-envelope"></i>
                        </router-link>
                    </li>
                </ul>
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

    .nav-container{
        box-shadow: 2px 2px 2px rgba(0,0,0,.3);
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

    ul {
        list-style: none;
    }

    li {
        display: inline;
        padding:  5px 15px;
        font-size: 1.8em;
    }

    i{
        color: #1d3557;
     }
    
    i:hover {
        color: #e63946;
    }
</style>