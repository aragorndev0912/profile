<template>
    <div id="portfolio" class="col-12">
        <h5 class="title">Portfolio</h5>
        <div class="row">
            <div class="col-12">
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor 
                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 
                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure 
                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt 
                    mollit anim id est laborum.
                </p>
            </div>

            <Task v-for="task in tasks" :key="task.id" :id="task.id" :images="task.images" :title="task.title" :subtitle="task.subtitle" :description="task.description" :uri="task.uri"/>
            
        </div>
    </div>
</template>

<script>

import Task from './Task.vue'

export default {
    name:'Portfolio',
    components:{
        Task,
    },
    data:function() {
        return {
            tasks:[
                {
                    id:0,
                    title:'amaia-vm',
                    subtitle:'Rust',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'https://github.com/aragorndev0912/amaia-vm',
                    images:['images/background.jpg'],
                },
                {
                    id:1,
                    title:'RPN Notation',
                    subtitle:'Rust',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'https://github.com/aragorndev0912/rpn',
                    images:['images/background.jpg', 'images/background.jpg'],
                },
                {
                    id:2,
                    title:'Beverly-lang',
                    subtitle:'ANSI C',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'https://github.com/aragorndev0912/beverly-lang',
                    images:['images/background.jpg', 'images/background.jpg'],
                },
                {
                    id:3,
                    title:'RAY2D Engine',
                    subtitle:'ANSI C',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'https://github.com/aragorndev0912/Ray2D',
                    images:['images/background.jpg', 'images/background.jpg'],
                },
                {
                    id:4,
                    title:'Hireme Page',
                    subtitle:'React',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'http://hireme.center/',
                    images:['images/background.jpg'],
                },
                {
                    id:5,
                    title:'Venepress',
                    subtitle:'React',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'https://venepress.com/',
                    images:['images/background.jpg', 'images/background.jpg'],
                },
                {
                    id:6,
                    title:'Progracademy Page',
                    subtitle:'HTML',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'http://www.progracademy.org/',
                    images:['images/background.jpg', 'images/background.jpg'],
                },
                {
                    id:7,
                    title:'Progracademy Admin',
                    subtitle:'PHP',
                    description:`Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.`,
                    uri:'http://www.progracademy.org/prg-test/',
                    images:['images/background.jpg', 'images/background.jpg'],
                },
            ],
        }
    }
}
</script>

<style scoped>
    @import '../assets/css/Portfolio.css';
</style>