<template>
    <div class="expertise-description">
        <p class="ed-title">{{title}}</p>
        <p class="ed-description" v-html="description"></p>
    </div>
</template>

<script>
export default {
    name:'ExpertiseDescription',
    props:['title', 'description']
}
</script>

<style>
    @import '../assets/css/ExpertiseDescription.css';
</style>