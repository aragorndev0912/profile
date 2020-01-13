<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" id="about-me" class="col-12"> 
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Algo sobre mi...</h5>
        <p class="text">
            Soy un desarrollador de software que siente un gran gusto por la programación de 
            intérpretes, compiladores y videojuegos utilizando el lenguaje <strong>C</strong>, actualmente estoy 
            desarrollando un interprete para un lenguaje de programación llamado 
            <a class="about-link" href="https://github.com/aragorndev0912/beverly-lang" target="_blank">Beverly</a> escrito en <strong>ANSI C</strong>. <br/><br/>
            
            Me gusta la programación de videojuegos, para eso utilizo una librería de <strong>C</strong>
            llamada <a class="about-link" href="https://www.raylib.com/" target="_blank">Raylib</a>, desde que la conocí fue amor a primera vista,
            ya que, simplifica mucho escribir código y es relativamente fácil las construcciones de prototipos.<br/>
            <br/>

            A nivel laboral tengo experiencia tanto en Frontend como en Backend utilizando herramientas de <strong>Javascript</strong>
            como <strong>React</strong>, <strong>Vue</strong>, <strong>NestJS</strong> y <strong>Express</strong>, junto con bases de datos
            relacionales y no relacionales como <strong>PostgreSQL</strong> y <strong>MongoDB</strong>.    
        </p>

    </div>
</template>

<script>
export default {
    name:'AboutMe',
    props:['isGray'],
}
</script>

<style scoped>
@import '../assets/css/AboutMe.css';
</style>