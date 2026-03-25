<script setup>

</script>

<template>
<nav class="navbar">
    <div class="logo">
        <a href="#home">Kassim Attoumani</a> 
    </div>

    <ul class="nav-links">
        <li><a href="#about">À propos</a></li>
        <li><a href="#projets">Projets</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
</template>

<style scoped>
.navbar {
    display: flex;
    justify-content: space-between; 
    align-items: center;
    padding: 1.5rem 5%; 
    border-bottom: 1px solid #FFFFFF;
}

.nav-links {
    display: flex; 
    list-style: none;
    gap: 2rem;
    margin: 0;
    padding: 0;
    
}

.logo a {
    color: #FFFFFF;
    font-weight: bold;
    font-size: 1.3rem;
    text-decoration: none;
}

.nav-links a {
    text-decoration: none; 
    color: #FFFFFF; 
    font-weight: 500;
    font-size: 1.1rem;
}
</style>