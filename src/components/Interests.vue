<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}"  id="interests" class="col-12">
        <h5 class="gray-title">Intereses</h5>

        <Interest v-for="(interest, index) in interests" v-bind:key="index" :title="interest.title" :description="interest.description" />

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
                    description:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."
                },
                {
                    title:"Desarrollo de videojuegos",
                    description:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."
                },
                {
                    title:"Programacion de motores graficos",
                    description:"Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."
                },
            ]
        }
    }
}
</script>

<style scoped> 
    @import '../assets/css/Interests.css';
</style>