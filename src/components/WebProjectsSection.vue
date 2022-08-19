<!-- WEB PROJECTS SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 19, 2022
-->

<template>
    <h1>WEB PROJECTS</h1>
    <div class="card-wrap">
        <div class="item-container" v-for="content in contents" :key="content.id">
            <WebProjectsItem :items="content" />
        </div>
    </div>
</template>

<script setup>
import WebProjectsItem from './items/WebProjectsItem.vue'

const contents = [
    {
        id: 0,
        image: "atlas.png",
        title: "ATLAS DOOR REPAIR",
        a: 'https://atlasdoorrepair.com/',
        body: "WordPress was used to create and maintain this website. I worked on this client website for four years. Aside from web maintenance, I also did SEO for Atlas, and the majority of the target keywords ranked first to third in Google. I also worked on Atlas' Landing Pages for Marketing using Click Funnels."
    }, //END OF ATLAS
    {
        id: 1,
        image: "naperville.png",
        title: "NAPERVILLE SERVICE LIMO",
        a: 'https://www.napervilleservicelimo.com/',
        body: "Weebly was used to create and maintain this website. I worked on this client website for four years. Aside from web maintenance, I also did SEO for Naperville, and the majority of the target keywords ranked first to second in Google."
    }, //END OF NAPERVILLE
    {
        id: 3,
        image: "bitc.png",
        title: "BITC ROOF TILES",
        a: 'https://www.bitcrooftiles.com/',
        body: "WordPress was used to create and maintain this website. I worked on this client website for two years. Aside from web maintenance, I also did SEO for BITC, and the majority of the target keywords ranked first to third in Google."
    }, //END OF BITC
    {
        id: 4,
        image: "cardetail.png",
        title: "MY CAR DETAIL CHICAGO",
        a: 'https://www.mycardetailchicago.com/',
        body: "WordPress was used to create and maintain this website. I worked on this client website for four years. Aside from web maintenance, I also did SEO for Naperville, and the majority of the target keywords ranked third to fifth in Google."
    } //END OF MY CAR DETAIL
]; /*END OF CONST CONTENTS*/
</script>

<style scoped>

</style>