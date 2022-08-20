<!-- WEB PROJECTS ITEM SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 19, 2022
-->

<template>
    <!-- <div class="card-wrap"> -->
        <!-- <div class="card-item"> -->
            <div class="wrap-item">
                <img :src="require('@/assets/' + props.items.image)">
                <div class="web-name">{{ props.items.title }}</div>
                <a class="web-visit" :href="props.items.a" target="_blank">Visit Site</a>
                <p class="web-detail">{{ props.items.body }}</p>
            </div>
        <!-- </div> -->
    <!-- </div> -->
</template>

<script setup>
import { defineProps } from 'vue'

const props = defineProps ({
    items: Object
})

console.log(props.items)
</script>

<style scoped>

img {
    height: 150px;
    width: 150px;
    border-radius: 50%;
    border: 5px double var(--main-black);
}

.web-name {
    color: var(--main-pink);
	font-weight: 900;
	letter-spacing: 2px;
	text-transform: uppercase;
	font-size: 28px;
    text-shadow: 1px 0px 2px black;
	white-space: wrap;
    overflow: hidden;
    text-overflow: ellipsis;
}

.web-visit {
    color: var(--main-black);
	font-size: 12px;
	font-weight: 100;
	margin: 5px 0 10px;
    text-decoration: none;
}

.web-visit:hover {
    color: white;
    background-color: var(--main-pink);
}

.web-detail {
    font-size: 18px;
	line-height: 24px;
	color: var(--main-black);
}

</style>