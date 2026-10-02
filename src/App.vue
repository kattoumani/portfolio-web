<template>
  <TheNavBar/>
  <HeroSection/>
  <AboutSection/>
  <SkillSection/>
</template>

<script setup>
import TheNavBar from './components/TheNavBar.vue';
import HeroSection from './components/HeroSection.vue';
import AboutSection from './components/AboutSection.vue';
import SkillSection from './components/SkillSection.vue';

</script>

<style>
body {
  font-family: "Space Grotesk", sans-serif;
  background-color: #F7F5EE; 
  color: #0f172a;
  margin: 0; 
  padding: 0;
}
  
</style>
