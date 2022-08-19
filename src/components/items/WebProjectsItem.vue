<!-- WEB PROJECTS ITEM SECTION
    WRITTEN BY: TRISHIA ANN CABUANG
    DATE: AUGUST 19, 2022
-->

<template>
    <div class="card-item">
        <div class="card-inner">
            <img :src="require('@/assets/' + props.items.image)">
            <div class="web-name">{{ prop.items.title }}</div>
            <a :href="prop.item.a" target="_blank">Visit Site</a>
            <p class="web-detail">{{ props.items.body }}</p>
        </div>
    </div>
</template>

<script>
import { defineProps } from 'vue'

const props = defineProps ({
    items: Object
})

console.log(props.items)
</script>

<style scoped>

</style>