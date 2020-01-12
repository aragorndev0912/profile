<template>
    <div id="information-section" class="col-md-6 col-12" :style="{margin:'0', padding:'0'}">
        <AboutMe :isGray="true" />
        <Skills :isGray="false"/>
        <Interests :isGray="true"/>
        <Experience :isGray="false"/>
        <Portfolio :isGray="true"/>
        <Education :isGray="false"/>
        <Expertise :isGray="true"/>
        <Contact :isGray="false"/>
    </div>
</template>

<script>

import AboutMe from './AboutMe.vue'
import Expertise from './Expertise.vue'
import Skills from './Skills.vue'
import Experience from './Experience.vue'
import Education from './Education.vue'
import Interests from './Interests.vue'
import Portfolio from './Portfolio.vue'
import Contact from './Contact.vue'

export default {
    name:'InformationSection',
    components:{
        AboutMe,
        Expertise,
        Skills,
        Experience,
        Education,
        Interests,
        Portfolio,
        Contact,
    }
}
</script>

<style scoped> 
    @import '../assets/css/InformationSection.css';
</style>