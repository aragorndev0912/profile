<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}"  id="experience" class="col-12">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Experiencia profesional</h5>
        <Information 
            date="2013 - 2014"
            title="Analista programador"
            work="Professional Evaluations Solutions"
            country="Venezuela"
            :activities="anincubator"
        />

        <Information 
            date="2016 - 2017"
            title="Analista programador"
            work="Novared"
            country="Venezuela"
            :activities="[]"
        />

        <Information 
            date="2019 - Presente"
            title="Desarrollador Backend y Frontend"
            work="Anincubator"
            country="Venezuela"
            :activities="[]"
        />

    </div>
</template>

<script>

import Information from './Information.vue'

export default {
    name:'Experience',
    props:['isGray'],
    components:{
        Information
    },
    data:function() {
        return {
            anincubator: [
                `- Migración de datos entre AWS y Youtube utilizando Python.`,
                `- Desarrollo de servicios utilizando Ruby On Rails con Pruebas en Postman.`,
                `- Uso de la Api de <strong class="info-span">Amazon S3</strong> para despliegue de ficheros.`,
                `- Creación de endpoints en NestJS con TypeScript y pruebas con Insomnia.`,
                `- Creación de endpoints con C#.`,
                `- <strong class="info-span">Lenguajes:</strong> Ruby, TypeScript, Python.`,
                `- <strong class="info-span">Bases de Dato:</strong> PostgreSQL, MongoDB.`,
                `- <strong class="info-span">Framework / Librerías:</strong> Ruby on Rails, React, NestJS.`,
                `- <strong class="info-span">Infraestructura:</strong> Amazon S3.`,
            ],
        }
    },

}
</script>

<style scoped>
    @import '../assets/css/Experience.css'
</style>