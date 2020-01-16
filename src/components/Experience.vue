<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}"  id="experience" class="col-12">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Experiencia profesional</h5>
        <Information 
            date="2013 - 2014"
            title="Analista programador"
            work="Professional Evaluations Solutions"
            country="Venezuela"
            :activities="pes"
        />

        <Information 
            date="2016 - 2017"
            title="Analista programador"
            work="Novared"
            country="Venezuela"
            :activities="novared"
        />

        <Information 
            date="2019 - Presente"
            title="Desarrollador Backend y Frontend"
            work="Anincubator"
            country="Venezuela"
            :activities="anincubator"
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
            pes:[
                `- Maquetación de ventanas con Bootstrap.`,
                `- Implementación de estilos con CSS y LESS.`,
                `- Desarrollo de servicios utilizando <strong>CakePHP</strong> con pruebas en Postman.`,
                `- <strong class="info-span">Bases de Datos:</strong> PostgreSQL, MySQL.`,

            ],
            novared: [
                `- Desarrollo de servicios utilizando <strong>Django</strong> con Pruebas en Postman.`,
                `- <strong class="info-span">Lenguajes:</strong> PHP, Javascript, Python.`,
                `- <strong class="info-span">Bases de Datos:</strong> PostgreSQL, MySQL.`,
                `- <strong class="info-span">Framework / Librerías:</strong> Django, CakePHP.`,
            ],
            anincubator: [
                `- Migración de datos entre <strong>AWS</strong> y <strong>Youtube</strong> utilizando Python.`,
                `- Desarrollo de servicios utilizando Ruby On Rails con Pruebas en Postman.`,
                `- Uso de la Api de <strong class="info-span">Amazon S3</strong> para despliegue de ficheros.`,
                `- Creación de endpoints en NestJS con TypeScript y pruebas con Insomnia.`,
                `- Backend .NET Framework.`,
                `- <strong class="info-span">Lenguajes:</strong> Ruby, TypeScript, Python.`,
                `- <strong class="info-span">Bases de Datos:</strong> PostgreSQL, MongoDB.`,
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