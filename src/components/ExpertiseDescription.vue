<template>
    <div class="expertise-description">
        <p :class="(isGray) ? 'ed-gray-title' : 'ed-title'">{{title}}</p>
        <p class="ed-description" v-html="description"></p>
    </div>
</template>

<script>
export default {
    name:'ExpertiseDescription',
    props:['title', 'description', 'isGray'],
}
</script>

<style>
    @import '../assets/css/ExpertiseDescription.css';
</style>