<template>
    <div id="education" class="col-12">
        <h5 class="title">Educación</h5>

        <Information 
            date="2002 - 2006"
            title="Primaria"
            work="U.E La Rosaleda"
            country="Venezuela"
        />

        <Information 
            date="2002 - 2007"
            title="Bachiller en Ciencias"
            work="U.E Liceo Militarizado Monseñor Arias"
            country="Venezuela"
        />

        <Information 
            date="2015"
            title="Certificado Programación con PHP-MySQL"
            work="Universidad Central de venezuela (UCV)"
            country="Venezuela"
        />

        <Information 
            date="2015"
            title="Certificado Programación con Java"
            work="Universidad Central de venezuela (UCV)"
            country="Venezuela"
        />

        <Information 
            date="2010 - 2019"
            title="Ingeniería en Informática"
            work="Universidad Católica Andrés Bello (UCAB)"
            country="Venezuela"
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