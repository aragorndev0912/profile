<template>
    <div id="hello">
        <span id="title">{{title}}</span>
        <br/>
        <span id="subtitle">{{subtitle}}</span>
    </div>
</template>

<script>
export default {
    name:'Hello',
    props:['title', 'subtitle'],
}
</script>

<style scoped>
@import '../assets/css/Hello.css';
</style>