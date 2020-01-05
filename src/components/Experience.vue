<template>
    <div id="experience" class="col-12">
        <h5 class="gray-title">Work Experience</h5>
        <Information 
            date="2015 - Present"
            title="HEAD OF MARKET RESEARCH"
            work="Computer & Motor Ltd."
            country="United Kingdom, London"
        />

        <Information 
            date="2012 - 2015"
            title="MEDIA ANALYST"
            work="BizzNiss"
            country="United Kingdom, London"
        />

        <Information 
            date="2010 - 2012"
            title="BUDGET ADMINISTRATOR"
            work="Somsom LLC"
            country="United Kingdom, London"
        />

    </div>
</template>

<script>

import Information from './Information.vue'

export default {
    name:'Experience',
    components:{
        Information
    }
}
</script>

<style scoped>
    @import '../assets/css/Experience.css'
</style>