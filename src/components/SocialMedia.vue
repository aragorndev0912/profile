<template>
        <a v-bind:href="_url" target="_blank">
    <span class="social-media">
            <i v-if="icon === 'linkedin'" class="fab fa-linkedin fa-2x"></i>
            <i v-if="icon === 'stack-overflow'" class="fab fa-stack-overflow fa-2x"></i>
            <i v-if="icon === 'git'" class="fab fa-github fa-2x"></i>
    </span>    
        </a>
</template>

<script>
export default {
    name:'SocialMedia',
    props:['icon', '_url'],
}
</script>

<style scoped>
/* <a href=""><i class="my-icon fab fa-linkedin fa-stack-2x"></i></a>*/
    @import '../assets/css/SocialMedia.css';
</style>