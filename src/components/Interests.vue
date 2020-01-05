<template>
    <div id="interests" class="col-12">
        <h5 class="gray-title">Interest</h5>

        <Interest 
            title="BOOKS"
            description="Proactively extend market-driven e-tailers rather than enterprise-wide supply chains. Collaboratively embrace 24/7 processes rather than adaptive users. Seamlessly monetize alternative e-business."
        />

        <Interest 
            title="SPORTS"
            description="Assertively grow optimal methodologies after viral technologies. Appropriately develop frictionless technology for adaptive functionalities. Competently iterate functionalized networks for best-of-breed services."
        />

        <Interest 
            title="ART"
            description="Dramatically utilize superior infomediaries whereas functional core competencies. Enthusiastically repurpose synergistic vortals for customer directed portals. Interactively pursue sustainable leadership via."
        />

    </div>
</template>

<script>

import Interest from './Interest.vue'

export default {
    name:'Interests',
    components:{
        Interest,
    }
}
</script>

<style scoped> 
    @import '../assets/css/Interests.css';
</style>