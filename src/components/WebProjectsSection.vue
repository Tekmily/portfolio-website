<!-- WEB PROJECTS SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 19, 2022
-->

<template>
    <h1>WEB PROJECTS</h1>
    <div id="card-wrap">
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
        body: "This website was built with WordPress. She worked on this client website for 4 years . Through SEO, most target keywords for this site ranked first to third in Google. She also worked on site's ClickFunnels landing pages."
    }, //END OF ATLAS
    {
        id: 1,
        image: "naperville.png",
        title: "NAPERVILLE SERVICE LIMO",
        a: 'https://www.napervilleservicelimo.com/',
        body: "This website was made with Weebly. She worked on this client website for 4 years. Through SEO, most target keywords for this site ranked first to second in Google. She also worked on site's social media page."
    }, //END OF NAPERVILLE
    {
        id: 3,
        image: "bitc.png",
        title: "BITC ROOF TILES",
        a: 'https://www.bitcrooftiles.com/',
        body: "This website was built with WordPress. She worked on this client website for 2 years. Through SEO, most target keywords for this site ranked first to third in Google. She also worked on site's social media page."
    }, //END OF BITC
    {
        id: 4,
        image: "cardetail.png",
        title: "MY CAR DETAIL CHICAGO",
        a: 'https://www.mycardetailchicago.com/',
        body: "This website was built with WordPress. She worked on this client website for 4 years. Through SEO, most target keywords for this site ranked third to fifth in Google. She also worked on site's social media page."
    } //END OF MY CAR DETAIL
]; /*END OF CONST CONTENTS*/
</script>

<style scoped>
#card-wrap {
    display: flex;
    justify-content: center;
    align-items: flex-start;
    gap: 20px;
    flex-wrap: wrap;
}
.item-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: var(--main-gray);
    width: clamp(100px, 50%, 450px);
    height: clamp(400px, 40%, 1200px);
    position: relative;
    border-radius: 4px;
    padding: 20px;
}

.item-container > * {
    padding: 10px;
}

.item-container:hover {
    background: var(--sub-pink);
    color: #fff;
    box-shadow: 0px 0px 11px 5px #000000;
}
</style>