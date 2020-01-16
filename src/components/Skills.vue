<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" id="skills" class="col-12">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Habilidades</h5>

        <h6 class="title-skill">+ Lenguajes de programacion:</h6>
        <Skill title="ANSI C" size="90" />        
        <Skill title="Python" size="70" />        
        <Skill title="Javascript" size="80" />      
        <Skill title="Rust" size="40" />        
        <br/>  
        <h6 class="title-skill">+ Frameworks, librerias y plataformas:</h6>
        <Skill title="Node" size="90" />        
        <Skill title="Vue" size="60" />        
        <Skill title="Django" size="80" />        
        <Skill title="Firebase" size="80" />        

        <br/>  
        <h6 class="title-skill">+ Bases de datos:</h6>
        <Skill title="MongoDB" size="90" />        
        <Skill title="PostgreSQL" size="90" />        

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