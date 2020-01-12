<template>
    <div id="image-section" class="col-md-6 col-12">

        <img id="aragorn" class="img-fluid" src="../assets/images/aragorn.png">

        <Hello 
            title="Hola, soy Franklin Morales!" 
            subtitle="ANSI C, Python, Vue and React developer."
        />

        <SocialMedia _url="https://www.linkedin.com/in/franklin-jose-morales-marquez-827554189/" icon="linkedin" />
        <SocialMedia _url="https://es.stackoverflow.com/users/141647/aragorndev0912" icon="stack-overflow" />
        <SocialMedia _url="https://github.com/aragorndev0912" icon="git" />

    </div>
</template>

<script>

import Hello from './Hello.vue'
import SocialMedia from './SocialMedia.vue'

export default {
    name:'ImageSection',
    components:{
        Hello,
        SocialMedia,
    }
}
</script>

<style scoped>
@import '../assets/css/ImageSection.css';
</style>