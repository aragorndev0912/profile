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
                    title:"Desarrollo de interpretes y compiladores",
                    description:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. text of the printing and typesetting industry."
                },
                {
                    title:"Desarrollo de videojuegos",
                    description:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. text of the printing and typesetting industry."
                },
                {
                    title:"Programacion de motores graficos",
                    description:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. text of the printing and typesetting industry."
                },
            ]
        }
    }
}
</script>

<style scoped> 
    @import '../assets/css/Interests.css';
</style>