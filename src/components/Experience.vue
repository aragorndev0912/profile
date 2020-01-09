<template>
    <div id="experience" class="col-12">
        <h5 class="gray-title">Experiencia profesional</h5>
        <Information 
            date="2013 - 2014"
            title="Analista programador"
            work="Professional Evaluations Solutions"
            country="Venezuela"
        />

        <Information 
            date="2016 - 2017"
            title="Analista programador"
            work="Novared"
            country="Venezuela"
        />

        <Information 
            date="2019 - Presente"
            title="Desarrollador Backend y Frontend"
            work="Anincubator"
            country="Venezuela"
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