<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" class="col-12 expertise">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Proyectos Sociales</h5>

        <div class="row">
            <div class="col-12 col-sm-6" v-for="(expertise, index) in expertises" v-bind:key="index">
                <ExpertiseDescription :isGray="isGray"  :title="expertise.title" :description="expertise.description" />
            </div>
        </div>
    </div>
</template>

<script>

import ExpertiseDescription from './ExpertiseDescription.vue'

export default {
    name:'Expertise',
    props:['isGray'],
    components:{
        ExpertiseDescription,
    },
    data:function() {
        return {
            expertises:[
                
                {
                    title:"Progracademy",
                    description:`Diseñador y programador de la página web para la iniciativa Progracademy: <br/><br/>link: <a class="ed-link" href="http://www.progracademy.org/" target="_blank">progracademy.org</a>`
                },
                {
                    title:"Clases de programacion",
                    description:`Dicté por unos meses clases de algoritmos y programación de forma gratuita en la casa de la cultura de mi municipio.`
                },
            ],
        }
    }

}
</script>

<style scoped>
    @import '../assets/css/Expertise.css';
</style>