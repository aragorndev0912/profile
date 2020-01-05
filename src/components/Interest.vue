<template>
    <div class="col-12 interest">
        <h6 class="int-title">{{title}}</h6>
        <p class="int-description">{{description}}</p>
    </div>
</template>

<script>
export default {
    name:'Interest',
    props:['title', 'description'],
}
</script>

<style scoped>
    @import '../assets/css/Interest.css';
</style>