<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" id="about-me" class="col-12"> 
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Algo sobre mi...</h5>
        <p class="text">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum 
        has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley 
        of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also 
        the leap into electronic typesetting, remaining essentially unchanged.
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