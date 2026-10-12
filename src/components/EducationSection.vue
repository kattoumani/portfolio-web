<template>
    <div class="education-section" id="education">
    <h1>Formation</h1>
    <div class="cards-container">
        <EducationCard v-for="edu in educations"
        :key="edu.course"
        :course="edu.course"
        :institution="edu.institution"
        :city="edu.city"
        :dateStart="edu.dateStart"
        :dateEnd="edu.dateEnd"
        :imageSrc="edu.imageSrc"
        />
    </div>
    </div>
</template>

<script setup>
import EducationCard from './EducationCard.vue';
import logoESGI from '@/assets/images/esgi.png';
import logoGuyChauvet from '@/assets/images/lycee-guy-chauvet.jpg';
import logoJeanMoulin from '@/assets/images/lycee-jean-moulin.png';


const educations = [
    {
        "course": "BTS SIO (Service informatiques aux organisations) - Option SLAM",
        "institution": "Lycée Guy Chauvet", 
        "city": "Loudun", 
        "dateStart": "Septembre 2022", 
        "dateEnd": "Juillet 2024",
        "imageSrc": logoGuyChauvet
    },
]

</script>

<style scoped>
.education-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
    padding-top: 150px;
}

.cards-container {
    display: flex;
    flex-direction: row;
    gap: 2rem;
}

h1 {
    text-align: center;
    font-size: 2.5rem;
}
    
</style>