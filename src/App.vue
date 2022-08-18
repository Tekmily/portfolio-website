<!--PORTFOLIO WEBSITE
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE WRITTEN: AUGUST 18, 2022
    VERSION: 1.0.2022
-->

<template>
  <section id="navigation-section">
    <NavigationSection/>
  </section>
  <section id="header-section">
    <HeaderSection />
  </section>
    <section id="about-section">
    <AboutSection />
  </section>
  <section id="projects-section">
    <ProjectsSection />
  </section>
  <section id="contact-section">
    <ContactSection />
  </section>

</template>

<script setup>
import NavigationSection from './components/NavigationSection.vue'
import HeaderSection from './components/HeaderSection.vue'
import AboutSection from './components/AboutSection.vue'
import ProjectsSection from './components/ProjectsSection.vue'
import ContactSection from './components/ContactSection.vue'
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 30px;
}

:root {
  --main-pink: rgba(245, 143, 124, 1);
  --main-black: rgba(44, 43, 48, 1);
  --main-gray: rgba(214, 214, 214, 1);
}

body {
  background-color: var(--main-black);
}

body h1, h2, h3 {
  color: var(--main-pink);
}

body p {
  color: var(--main-gray);
}
</style>
