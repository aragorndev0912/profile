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
                    description:'descripcion#0',
                    uri:'https://github.com/aragorndev0912/amaia-vm',
                    images:['images/girl.jpg', 'images/img1.jpg'],
                },
                {
                    id:1,
                    title:'RPN Notation',
                    subtitle:'Rust',
                    description:'descripcion#1',
                    uri:'https://github.com/aragorndev0912/rpn',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
                {
                    id:2,
                    title:'Beverly-lang',
                    subtitle:'ANSI C',
                    description:'descripcion#2',
                    uri:'https://github.com/aragorndev0912/beverly-lang',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
                {
                    id:3,
                    title:'RAY2D Engine',
                    subtitle:'ANSI C',
                    description:'descripcion#3',
                    uri:'https://github.com/aragorndev0912/Ray2D',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
                {
                    id:4,
                    title:'Hireme Page',
                    subtitle:'React',
                    description:'descripcion#4',
                    uri:'http://hireme.center/',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
                {
                    id:5,
                    title:'Venepress',
                    subtitle:'React',
                    description:'descripcion#5',
                    uri:'https://venepress.com/',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
                {
                    id:6,
                    title:'Progracademy Page',
                    subtitle:'HTML',
                    description:'descripcion#6',
                    uri:'http://www.progracademy.org/',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
                {
                    id:7,
                    title:'Progracademy Admin',
                    subtitle:'PHP',
                    description:'descripcion#7',
                    uri:'http://www.progracademy.org/prg-test/',
                    images:['images/img0.jpg', 'images/img1.jpg'],
                },
            ],
        }
    }
}
</script>

<style scoped>
    @import '../assets/css/Portfolio.css';
</style>