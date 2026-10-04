<template>
    <div class="experience-card">
        <h3>{{ jobTitle }}</h3>
        <img :src="companyLogo" :alt="companyName"><p>{{ companyName }}, {{ cityName }} | {{ startDate }} - {{ endDate }}</p>
        <ul class="missions">
            <li v-for="mission in missions" :key="mission">{{ mission }}</li>
        </ul>
        <ul class="technologies">
            <li v-for="technologie in technologies" :key="technologie">{{ technologie }}</li>
        </ul>
    </div>
</template>

<script setup>
defineProps({
    jobTitle: String,
    companyName: String,
    companyLogo: String,
    cityName: String,
    startDate: String,
    endDate: String,
    missions: Array,
    technologies: Array
});
</script>

<style scoped>

.experience-card {
    position: relative;
    width: 100%;
    max-width: 1000px;
    border: 1px solid;
    padding: 15px;
    border-radius: 3%;
}

.missions li {
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
    border: 2px solid #DCDADA;
    border-radius: 15%;
    padding: 5px;
}

img {
    position: absolute;
    top: 15px;
    right: 15px;
    width: 70px;
}
</style>