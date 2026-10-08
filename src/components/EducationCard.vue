<template>
    <div class="education-card">
        <h2>{{ course }}</h2>
        <p>{{ institution }}, {{ city }} {{ dateStart }} - {{ dateEnd }}</p>
        <img :src="imageSrc" :alt="imageSrc">
    </div>
</template>

<script setup>
defineProps({
    course: String,
    institution: String,
    city: String,
    dateStart: String,
    dateEnd: String,
    imageSrc: String
})

</script>

<style scoped>
.education-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 400px;
    border: 2px solid black;
    border-radius: 12px;
    padding: 5px
}

img {
    width: 150px;
}

    
</style>