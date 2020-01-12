<template>
    <div id="information" class="col-12">
        <span class="info-date">{{date}}</span>
        <p class="info-title">{{title}}</p>
        <p class="info-text">
            <strong>{{work}}</strong>
            <br/>
            {{country}}
        </p>
        <div v-if="activities.length > 0">
            <label class="info-actividades">+ Actividades:</label>
            <ul>
                <li class="info-li" v-for="(activity, index) in activities" :key="index" v-html="activity"></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name:'Information',
    props:['date', 'title', 'work', 'country', 'activities'],
}
</script>

<style scoped>
    @import '../assets/css/Information.css';
</style>