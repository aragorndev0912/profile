<template>
    <div id="interests" class="col-12">
        <h5 class="gray-title">Intereses</h5>

        <Interest v-for="(interest, index) in interests" v-bind:key="index" :title="interest.title" :description="interest.description" />

    </div>
</template>

<script>

import Interest from './Interest.vue'

export default {
    name:'Interests',
    components:{
        Interest,
    },
    data:function() {
        return {
            interests:[
                {
                    title:"Desarrollo de interpretes y compiladores",
                    description:"Proactively extend market-driven e-tailers rather than enterprise-wide supply chains. Collaboratively embrace 24/7 processes rather than adaptive users. Seamlessly monetize alternative e-business."
                },
                {
                    title:"Desarrollo de videojuegos",
                    description:"Assertively grow optimal methodologies after viral technologies. Appropriately develop frictionless technology for adaptive functionalities. Competently iterate functionalized networks for best-of-breed services."
                },
                {
                    title:"Programacion de motores graficos",
                    description:"Dramatically utilize superior infomediaries whereas functional core competencies. Enthusiastically repurpose synergistic vortals for customer directed portals. Interactively pursue sustainable leadership via."
                },
            ]
        }
    }
}
</script>

<style scoped> 
    @import '../assets/css/Interests.css';
</style>