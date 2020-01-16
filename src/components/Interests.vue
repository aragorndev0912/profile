<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}"  id="interests" class="col-12">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Intereses</h5>

        <Interest :isGray="isGray" v-for="(interest, index) in interests" v-bind:key="index" :title="interest.title" :description="interest.description" />

    </div>
</template>

<script>

import Interest from './Interest.vue'

export default {
    name:'Interests',
    props:['isGray'],
    components:{
        Interest,
    },
    data:function() {
        return {
            interests:[
                {
                    title:"+ Desarrollo de compiladores e intérpretes",
                    description:"Actualmente me encuentro desarrollando un intérprete en ANSI C."
                },
                {
                    title:"+ Desarrollo de videojuegos",
                    description:`Es un hobbie que disfruto mucho, utilizo la librería <a class="about-link" href="https://www.raylib.com/" target="_blank">Raylib</a> para realizar todas mis pruebas.`,
                },
                {
                    title:"+ Desarrollo web.",
                    description:"Disfruto mucho con el desarrollo de single pages applications utilizando <strong>Vue</strong>, <strong>NestJS</strong> y <strong>Firebase</strong>"
                },
            ]
        }
    }
}
</script>

<style scoped> 
    @import '../assets/css/Interests.css';
</style>