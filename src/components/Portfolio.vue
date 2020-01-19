<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" id="portfolio" class="col-12">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Portfolio</h5>
        <div class="row">
            <div class="col-12">
                <p class="portafolio-text">
                    A continuación, presento algunos de mis trabajos personales y proyectos sociales que he realizado 
                    en el transcurso del tiempo, algunos tienen links a articulos que he escrito en Linkedin y todos 
                    tienen el repositorio para poder descargar el código fuente.
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
    props:['isGray'],
    components:{
        Task,
    },
    data:function() {
        return {
            tasks:[
                {
                    id:0,
                    title:'Amaia virtual machine',
                    subtitle:'Rust (artículo)',
                    description:`<strong>Amaia virtual machine (AVM)</strong>, es una pequeña maquina virtual que ejecuta instrucciones en números
                    hexadecimales, la idea era desarrollar un compilador para un lenguaje de programación inventado, en este caso <strong>el lenguaje Amaia</strong>.
                    El compilador generaría instrucciones hexadecimales como código objeto y esta sería ejecutadas por la <strong>AVM</strong>.<br/><br/>
                    
                    La máquina virtual fue programada en Rust, aquí dejo los enlaces a la publicación hecha en linkedin y al codigo fuente.
                    `,
                    uri:[{title:'Github', uri:'https://github.com/aragorndev0912/amaia-vm'}, {title:'Artículo en Linkedin', uri:'https://www.linkedin.com/pulse/tiny-virtual-machine-franklin-jose-morales-marquez/'}],
                    images:['images/amaia.jpg'],
                },
                {
                    id:1,
                    title:'RPN para Amaia-lang.',
                    subtitle:'Rust (artículo)',
                    description:`El intérprete del lenguaje de programación Amaia (en algún momento me pondré a programarlo), internamente utilizará la Notación 
                    Polaca Inversa. para la evaluación de las expresiones aritméticas. Se desarrolló un módulo escrito en el lenguaje Rust que permite 
                    evaluar expresiones definidas dentro de un fichero de texto con extensión .ope, escritas utilizando la Notación Algebraica, 
                    para luego ser convertidas a expresiones definidas bajo la Notación Polaca Inversa y al final evaluarlas y obtener el resultado 
                    de la operaciones.`,
                    uri:[{title:'Github', uri:'https://github.com/aragorndev0912/rpn'}, {title:'Artículo en Linkedin', uri:'https://www.linkedin.com/pulse/evaluaci%C3%B3n-aritm%C3%A9tica-para-un-compilador-o-int%C3%A9rprete-franklin-jose/'}],
                    images:['images/rpn.jpg'],
                },
                {
                    id:2,
                    title:'Overflow Engine.',
                    subtitle:'ANSI C',
                    description:`Ray2D (Overflow Engine) es un editor de mapas que estoy desarrollando para la creación de un videojuego similar al <strong>Wolfenstein 3D</strong>, lo estoy
                    programando utilizando una librería de C bastante simple para el prototipado y la programación de videojuegos, Raylib.
                    Tengo este proyecto algo abandonado porque ahorita estoy con mi intérprete <a class="about-link" href="https://github.com/aragorndev0912/beverly-lang" target="_blank">Beverly</a>, 
                    una vez lo acabe, retomaré este proyecto.`,
                    uri:[{title:'Github Ray2D', uri:'https://github.com/aragorndev0912/Ray2D'}],
                    images:['images/ray2d_0.jpg', 'images/ray2d_1.jpg'],
                },
            ],
        }
    }
}
</script>

<style scoped>
    @import '../assets/css/Portfolio.css';
</style>