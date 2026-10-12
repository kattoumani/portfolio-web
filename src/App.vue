<template>
  <TheNavBar/>
  <HeroSection/>
  <AboutSection/>
  <SkillSection/>
  <ExperienceSection/>
  <EducationSection/>
  <ProjectSection />
  <FooterSection />
</template>

<script setup>
import TheNavBar from './components/TheNavBar.vue';
import HeroSection from './components/HeroSection.vue';
import AboutSection from './components/AboutSection.vue';
import SkillSection from './components/SkillSection.vue';
import ExperienceSection from './components/ExperienceSection.vue';
import EducationSection from './components/EducationSection.vue';
import ProjectSection from './components/ProjectSection.vue';
import FooterSection from './components/FooterSection.vue';

</script>

<style>
* {
  box-sizing: border-box;
}

body {
    overflow-x: hidden;
}

body {
  font-family: "Space Grotesk", sans-serif;
  background-color: #F7F5EE; 
  color: #0f172a;
  margin: 0; 
  padding: 0;
}
  
</style>
