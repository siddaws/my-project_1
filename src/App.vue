<script setup>
import HeaderComp from './components/HeaderComp.vue';
import ProfileComp from './components/ProfileComp.vue';
import EducationComp from './components/EducationComp.vue';
import Skills from './components/Skills.vue';
import LanguageComp from './components/LanguageComp.vue';
</script>

<template>
  <HeaderComp />
  <ProfileComp />
  <EducationComp 
    title="Освіта" 
    subtitle="Комп'ютерна інженерія" 
    description="Київський електромеханічний коледж Київ, Україна" 
    dates="9/2021 - 7/2024" 
  />
  <EducationComp 
    title="Досвід роботи" 
    subtitle="Системний адміністратор" 
    description="- Київ, Україна" 
    dates="3/2024-7/2024" 
  />
  <Skills />
  <LanguageComp />
</template>

<style scoped>
@media (max-width: 768px) {
  .burger-menu {
    display: block;
  }
}

.burger-menu ul {
  display: none;
}

.burger-menu ul.open {
  display: block;
}
</style>