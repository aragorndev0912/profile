<template>
    <div class="col skill">
        <label :style="{fontWeight:'800', color:'#57606f'}">{{title}}</label>
        <div class="progress">
          <div class="progress-bar" role="progressbar" :style="{width: size+'%', backgroundColor:'#ff6348'}" :aria-valuenow="size" aria-valuemin="0" aria-valuemax="100">{{size}}%</div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Skill',
    props:['title', 'size'],
    
}
</script>

<style scoped>
    @import '../assets/css/Skill.css';
</style>