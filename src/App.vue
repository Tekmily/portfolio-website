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

  <section id="webprojects-section">
    <WebProjectsSection />
  </section>

  <section id="active-websites">
    <ActiveWebsites />
  </section>

  <section id="seo-results">
    <SeoResults />
  </section>

  <section id="contact-section">
    <ContactSection />
  </section>

</template>

<script setup>
import NavigationSection from './components/NavigationSection.vue'
import HeaderSection from './components/HeaderSection.vue'
import AboutSection from './components/AboutSection.vue'
import WebProjectsSection from './components/WebProjectsSection.vue'
import ActiveWebsites from './components/ActiveWebsites.vue'
import SeoResults from './components/SeoResults.vue'
import ContactSection from './components/ContactSection.vue'
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

:root {
  --main-pink: rgba(245, 143, 124, 1);
  --main-black: rgba(44, 43, 48, 1);
  --main-gray: rgba(214, 214, 214, 1);
  --sub-pink: rgba(242, 196, 206, 1);
}

html {
  scroll-behavior: smooth;
}

body {
  background-color: var(--main-black);
  text-align: center;

}

body h1, h2, h3 {
  color: var(--main-pink);
  font-weight: bold;
}

h1 {
  font-size: 48px;
}

h2 {
  font-size: 40px;
}

h3 {
  font-size: 32px;
}

p {
  color: var(--main-gray);
  font-size: 20px;
}

#navigation-section {
  position: sticky;
  z-index: 1;
  top: 0;
  padding: 1vw 2vw;
  background-color: var(--main-black) ;
  width: 100%;
  margin-left: -1vw;
}

#header-section {
  margin-left: -2vw;
  margin-right: -3vw;
}


</style>
