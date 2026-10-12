<template>
    <div class="project-section" id="projects">
    <h1>Projets</h1>
    <ProjectCard 
        v-for="pro in projects"
        :key="pro.projectTitle"
        :projectTitle="pro.projectTitle"
        :description="pro.description"
        :productions="pro.productions"
        :imageSrc="pro.imageSrc"
        :technologies="pro.technologies"
        :githubLink="pro.githubLink"
    />  
    </div>
</template>

<script setup>
import ProjectCard from './ProjectCard.vue';
import logoWebRadio from "@/assets/images/logo-web-radio.png";

const projects = [
    {
        projectTitle: "Portfolio",
        description: "Vitrine web professionnelle conçue pour présenter mon profil, mes compétences techniques et mes réalisations.",
        productions: [
            "Interface & UX : Conception d'une interface dynamique, responsive et accessible.", 
            "Architecture : Structure modulaire et propre pour faciliter la maintenance et les évolutions.",
            "Déploiement : Hébergement et intégration continue via Cloudflare et GitHub.",
        ],
        imageSrc: "",
        technologies: [
            "Vue.JS",
            "Git",
            "GitHub",
            "Cloudflare"
        ],
        githubLink: "https://github.com/kattoumani/portfolio-web"
    },

    {
        projectTitle: "WebRadio Lycée Guy Chauvet, Loudun",
        description: "Réalisation en équipe d'une solution web complète dédiée à la publication, l'écoute et la gestion des podcasts produits par le lycée.",
        productions: [
            "Gestion des médias & Lecteur audio : Intégration d'un lecteur audio et structuration du flux de lecture des podcasts.", 
            "Back-Office & Administration : Mise en place d'un espace d'administration sécurisé sous Symfony pour permettre à l'équipe de gérer les contenus, catégories et publications.",
            "Base de données : Conception du schéma relationnel (SQL)",
            "Workflow collaboratif : Utilisation rigoureuse de Git/GitHub pour le suivi de version, la résolution des conflits."
        ],
        imageSrc: logoWebRadio,
        technologies: [
            "HTML/CSS",
            "PHP Symfony",
            "PostgreSQL",
            "Apache",
            "Adminer",
        ],
        githubLink: "https://github.com/ben7821/WebRadio.git"
    }
]

</script>

<style scoped>
.project-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
    padding-top: 150px;
    padding-bottom: 100px;
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