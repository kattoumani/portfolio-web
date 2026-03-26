<script>

</script>

<template>
    <div>
        <section id="hero">
            <div class="presentation">
                <h1>Développeur Full Stack en alternance</h1>
                <p>Développeur Full Stack en alternance (PHP Symfony/Laravel & Vue.js | MVC & POO)
                    <br><br>
                    Futur étudiant en bachelor 3ème année à l'ESGI (rentrée septembre 2026) et passionné par l'architecture logicielle, 
                    je me spécialise en Développement Full Stack.<br><br>
                    
                    Bien que mon parcours soit marqué 
                    par une forte expertise en PHP et Symfony, je considère les langages comme 
                    des outils au service des enjeux métiers. <br><br>

                    Maîtrisant les environnements Linux/Docker et les outils de versioning, 
                    je suis ouvert à l'apprentissage de nouvelles stacks pour construire des 
                    solutions robustes et évolutives.
                </p>
                <div class="social-media-link">
                    <div><a href="https://www.linkedin.com/in/kassim-attoumani/" target="_blank"><img src="/images/linkedin.png" alt=""></a></div>
                    <div><a href="https://github.com/kattoumani" target="_blank"><img src="/images/github.png" alt=""></a></div>
                    <div><a href="https://gitlab.com/kattoumani" target="_blank"><img src="/images/gitlab.png" alt=""></a></div>
                </div>
            </div>
            <div class="profile-picture">
                <img src="/images/profile_picture.jpeg" alt="Photo de profil">
            </div>

        </section>
    </div>
</template>

<style scoped>
#hero {
    display: flex;
    padding-top: 100px;
    justify-content: center;
    gap: 5rem;
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