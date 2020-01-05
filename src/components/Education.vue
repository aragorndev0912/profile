<template>
    <div id="education" class="col-12">
        <h5 class="title">Education</h5>

        <Information 
            date="2010 - 2012"
            title="MA PRODUCT DESIGN"
            work="University of California"
            country="United Kingdom, London"
        />

        <Information 
            date="2007 - 2010"
            title="BUSINESS MARKETING COURSE"
            work="Royal Academy of Business"
            country="United Kingdom, London"
        />

        <Information 
            date="2002 - 2006"
            title="BA (HONS) DESIGN"
            work="University of Michigan"
            country="United Kingdom, London"
        />
        
    </div>
</template>

<script>

import Information from './Information.vue'

export default {
    name:'Education',
    components:{
        Information,
    }
}
</script>

<style scoped>
    @import '../assets/css/Education.css';
</style>