<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" id="skills" class="col-12">
        <h5 class="title">Habilidades</h5>

        <Skill title="ANSI C" size="100" />        
        <Skill title="React" size="90" />        
        <Skill title="Vue" size="100" />        
        <Skill title="Rust" size="70" />        
        <Skill title="MongoDB" size="90" />        
        <!--<Skill title="Django" size="90" />        
        <Skill title="PostgreSQL" size="90" />        -->

    </div>
</template>

<script>

import Skill from './Skill.vue'

export default {
    name:'Skills',
    props:['isGray'],
    components:{
        Skill,
    }
}
</script>

<style scoped> 
    @import '../assets/css/Skills.css';
</style>