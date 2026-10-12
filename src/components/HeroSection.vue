<template>
    <div>
        <section id="hero">
            <div class="presentation">
                <h1>Développeur informatique</h1>
                <p>
                    Développeur Informatique passionné par la conception et la maintenance d'applications web et logiciels. 
                    Spécialisé en PHP (Symfony/Laravel), JavaScript (Vue.js) et bases de données SQL, 
                    je maîtrise les environnements conteneurisés (Docker, Linux) pour construire des solutions performantes, 
                    robustes et adaptées aux besoins métiers. Disponible immédiatement.
                </p>
                <div class="social-media-link">
                    <div><a href="https://www.linkedin.com/in/kassim-attoumani/" target="_blank"><img src="@/assets/images/linkedin.png" alt=""></a></div>
                    <div><a href="https://github.com/kattoumani" target="_blank"><img src="@/assets/images/github.png" alt=""></a></div>
                    <div><a href="https://gitlab.com/kattoumani" target="_blank"><img src="@/assets/images/gitlab.png" alt=""></a></div>
                </div>
            </div>
            <div class="profile-picture">
                <img src="@/assets/images/profile_picture.jpeg" alt="Photo de profil">
            </div>

        </section>
    </div>
</template>

<script>

</script>

<style scoped>
#hero {
    display: flex;
    padding-top: 100px;
    justify-content: center;
    gap: 5rem;
    min-height: 100vh;
}

p {
    font-size: 1.2rem;
}

.presentation {
    width: 700px;
    height: 600px;
}

.presentation p {
    padding-bottom: 50px;
}

.profile-picture img {
    width: 350px;
    height: 350px;
    border-radius: 50%;
}

.social-media-link {
    display: flex;
    gap: 1.4rem;
    flex-direction: row;
    align-items: flex-end;
}

.social-media-link img {
    width: 40px;
    height: 40px;
}

</style>