<template>
    <div class="projects-card">
    <img v-if="imageSrc != ''" :src="imageSrc" :alt="projectTitle"><h1>{{ projectTitle }}</h1>
    <p>{{ description }}</p>
    <a :href="githubLink">Github</a>
    <ul class="productions">
        <li v-for="pro in productions" :key="pro.production">{{ pro }}</li>
    </ul>
    <ul class="technologies">
        <li v-for="tech in technologies" :key="tech.technologies">{{ tech }}</li>
    </ul>
    </div>
</template>

<script setup>
defineProps({
    projectTitle: String,
    description: String,
    productions: Array,
    imageSrc: String,
    technologies: Array,
    websiteLink: String,
    githubLink: String
});
</script>

<style scoped>
.projects-card {
    position: relative;
    width: 100%;
    max-width: 1000px;
    border: 1px solid;
    padding: 15px;
    border-radius: 12px;
}

.productions li {
    margin-bottom: 0.9rem;
}

.technologies {
    display: flex;
    flex-direction: row;
    list-style-type: none;
    gap: 1.5rem;
    border-radius: 2px solid black;
}

.technologies li {
    border: 2px solid black;
    border-radius: 12px;
    padding: 5px;
}

img {
    position: absolute;
    top: 15px;
    right: 15px;
    width: 70px;
}

@media (max-width: 768px) {
    .technologies {
        flex-wrap: wrap;
        gap: 0.8rem;
    }
}


</style>

