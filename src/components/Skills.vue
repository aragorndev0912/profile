<template>
    <div id="skills" class="col-12">
        <h5 class="title">Skills</h5>

        <Skill title="C/C++" size="90" />        
        <Skill title="Rust" size="20" />        
        <Skill title="JavaScript" size="80" />        
        <Skill title="TypeScript" size="70" />        

    </div>
</template>

<script>

import Skill from './Skill.vue'

export default {
    name:'Skills',
    components:{
        Skill,
    }
}
</script>

<style scoped> 
    @import '../assets/css/Skills.css';
</style>