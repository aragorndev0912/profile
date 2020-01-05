<template>
    <div id="information" class="col-12">
        <span class="info-date">{{date}}</span>
        <p class="info-title">{{title}}</p>
        <p class="info-text">
            <strong>{{work}}</strong>
            <br/>
            {{country}}
        </p>

    </div>
</template>

<script>
export default {
    name:'Information',
    props:['date', 'title', 'work', 'country'],
}
</script>

<style scoped>
    @import '../assets/css/Information.css';
</style>