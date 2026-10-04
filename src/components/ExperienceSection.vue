<template>
    <div class="experience-section" id="experience">
        <h1>Expériences</h1>
        <ExperienceCard 
            v-for="exp in experiences"
            :key="exp.companyName"
            :jobTitle="exp.jobTitle"
            :companyName="exp.companyName"
            :companyLogo="exp.companyLogo"
            :cityName="exp.cityName"
            :startDate="exp.startDate"
            :endDate="exp.endDate"
            :missions="exp.missions"
            :technologies="exp.technologies"
        />
    </div>
</template>

<script setup>
import ExperienceCard from './ExperienceCard.vue';
import logo6tm from '@/assets/images/6tm.png';
import logoSothogam from '@/assets/images/sothogam.png';
import logoPascalSauvetre from '@/assets/images/pascal-sauvetre.png';
import logoConseilDepartemental from '@/assets/images/conseil-departemental.png';

const experiences = [
    {
        jobTitle: "Développeur PHP Laravel",
        companyName: "Hegyd 6TM",
        companyLogo: logo6tm,
        cityName: "Beaucouzé",
        startDate: "Mars 2025",
        endDate: "Juillet 2025",
        missions: [
            "Conception d’un système de traitement automatisé de fichiers massifs (CSV/Excel de plus de 30k lignes) avec contrôle d'intégrité, insertion en base de données et gestion des statuts",
            "Création d'interfaces d'administration (Datatables) pour le suivi en temps réel des traitements, incluant logs d'erreurs, notifications e-mails et archivage.",
            "Rédaction de la documentation technique et réalisation de démonstrations auprès d’une équipe de 6 développeurs."
        ],
        technologies: [
            "Laravel", 
            "Git",
            "GitLab",
            "Docker",
            "Ubuntu",
            "PHP Storm"
        ]
    },

    {
        jobTitle: "Développeur PHP Symfony",
        companyName: "Groupe Sothogam",
        companyLogo: logoSothogam,
        cityName: " Mauzé-Thouarsais",
        startDate: "Janvier 2024",
        endDate: "Mars 2024",
        missions: [
            "Migration complète d'une application de pointage (Legacy PHP 5 vers Symfony 6) et conception de la nouvelle architecture de données MySQL.",
            "Création de formulaires pour la saisie des temps de travail et gestion des flux de données pour les collaborateurs du service commercial.",
            "Implémentation de l'authentification LDAP/Active Directory et automatisation de la récupération des données hiérarchiques (services, managers)."
        ],
        technologies: [
            "Symfony",
            "Bootstrap",
            "MySQL",
            "Debian",
            "VS Code"
        ]
    },

    {
        jobTitle: "Développeur Backend PHP",
        companyName: "Création de site par Ici - Pascal Sauvetre",
        companyLogo: logoPascalSauvetre,
        cityName: "Argentonnay",
        startDate: "Mai 2023",
        endDate: "Juin 2023",
        missions: [
            "Conception de formulaires dynamiques et automatisation de la collecte de données de devis",
            "Implémentation d' un moteur de création de PDF personnalisés (librairie FPDF) incluant la gestion de la mise en page.",
            "Automatisation de la génération de devis et transmission par e-mail au client et à la direction."
            ],
        technologies: [
            "PHP",
            "MySQL",
            "VS Code"
        ]
    },

    {
        jobTitle: "Développeur PHP Laravel",
        companyName: "Conseil départemental",
        companyLogo: logoConseilDepartemental,
        cityName: "Mamoudzou (Mayotte)",
        startDate: "Mai 2022",
        endDate: "Juin 2022",
        missions: [
            "Modernisation visuelle de la section Blog via le framework Bootstrap.",
            "Implémentation et configuration d' un éditeur WYSIWYG (ContentTools) pour simplifier la saisie de contenu riche par les utilisateurs.",
            "Création de templates d'articles dynamiques utilisant le moteur de rendu de Laravel, assurant une structure HTML propre et maintenable."
        ],
        technologies: [
            "Laravel",
            "Bootstrap",
            "VS Code"
        ]
    },
]


</script>

<style scoped>
.experience-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 100px;
    gap: 2rem;
    min-height: 100vh;
}

h1 {
    text-align: center;
    font-size: 2.5rem;
}
</style>