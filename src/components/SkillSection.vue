<template>
    <div class="skill-section" id="skills">
    <h1>Compétences</h1>
    <div class="card-container">

    <div class="skill border-bottom">
    <!-- Front-end -->
    <h2>Front-end</h2>
        <SkillCard :name="'HTML'" :imageSrc="logoHtml" :alt="HTML"/>
        <SkillCard :name="'CSS'" :imageSrc="logoCss" :alt="CSS"/>
        <SkillCard :name="'Javascript'" :imageSrc="logoJavascript" :alt="Javascript"/>
    </div>

    <!-- Back-end -->
    <div class="skill border-bottom">
    <h2>Back-end</h2>
        <SkillCard :name="'PHP'" :imageSrc="logoPhp" :alt="PHP"/>
        <SkillCard :name="'Java'" :imageSrc="logoJava" :alt="Java"/>
        <SkillCard :name="'C#'" :imageSrc="logoCsharp" :alt="CSharp"/>
    </div>

    <!-- Base de données -->

    <div class="skill border-bottom">
    <h2>Base de données</h2>
        <SkillCard :name="'PostgreSQL'" :imageSrc="logoPostgreSQL" :alt="PostgreSQL"/>
        <SkillCard :name="'MySQL'" :imageSrc="logoMySql" :alt="MySQL"/>
    </div>


    <!-- Framework -->

    <div class="skill border-bottom">
    <h2>Frameworks</h2>
        <SkillCard :name="'Symfony'" :imageSrc="logoSymfony" :alt="Symfony"/>
        <SkillCard :name="'Laravel'" :imageSrc="logoLaravel" :alt="Laravel"/>
        <SkillCard :name="'VueJs'" :imageSrc="logoVue" :alt="VueJs"/>
    </div>

    <!-- DevOps -->

    <div class="skill border-bottom">
    <h2>DevOps</h2>
        <SkillCard :name="'Debian'" :imageSrc="logoDebian" :alt="Debian"/>
        <SkillCard :name="'Fedora'" :imageSrc="logoFedora" :alt="Fedora"/>
        <SkillCard :name="'Bash'" :imageSrc="logoBash" :alt="Bash"/>
        <SkillCard :name="'Git'" :imageSrc="logoGit" :alt="Git"/>
        <SkillCard :name="'GitHub'" :imageSrc="logoGitHub" :alt="GitHub"/>
        <SkillCard :name="'GitLab'" :imageSrc="logoGitLab" :alt="GitLab"/>
        <SkillCard :name="'Docker'" :imageSrc="logoDocker" :alt="Docker"/>
    </div>
    </div>
    </div>

</template>

<script setup>
import SkillCard from './SkillCard.vue';
import logoHtml from '@/assets/images/html.png';
import logoCss from '@/assets/images/css.png';
import logoJavascript from '@/assets/images/javascript.png';
import logoPhp from '@/assets/images/php.png';
import logoJava from '@/assets/images/java.png';
import logoCsharp from '@/assets/images/csharp.png';
import logoPostgreSQL from '@/assets/images/postgresql.png';
import logoMySql from '@/assets/images/mysql.png';
import logoSymfony from '@/assets/images/symfony.png';
import logoLaravel from '@/assets/images/laravel.png';
import logoVue from '@/assets/images/vue.png';
import logoDebian from '@/assets/images/debian.png';
import logoFedora from '@/assets/images/fedora.png';
import logoBash from '@/assets/images/bash.png';
import logoGit from '@/assets/images/git.png';
import logoGitHub from '@/assets/images/github.png';
import logoGitLab from '@/assets/images/gitlab.png';
import logoDocker from '@/assets/images/docker.png';


</script>

<style scoped>
.skill-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 100px;
    gap: 5rem;
}

.card-container {
    display:flex;
    flex-direction: column;
    gap: 2rem;
}

.skill {
    display:flex;
    flex-direction: row;
    gap: 2rem;
}

h1 {
    text-align: center;
    font-size: 2.5rem;
}

.border-bottom {
    border-bottom: 1px solid #000000;
}
</style>