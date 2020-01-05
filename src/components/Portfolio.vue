<template>
    <div id="portfolio" class="col-12">
        <h5 class="title">Portfolio</h5>
        <div class="row">
            <Task id="0" title="Creative concepts" subtitle="domain.com" description="descripcion 0"/>
            <Task id="1" title="Customer focused" subtitle="domain.com" description="descripcion 1"/>
            <Task id="2" title="Management methodology" subtitle="domain.com" description="descripcion 2"/>
            <Task id="3" title="Market research" subtitle="domain.com" description="descripcion 3"/>
        </div>
    </div>


</template>

<script>

import Task from './Task.vue'

export default {
    name:'Portfolio',
    components:{
        Task,
    }
}
</script>

<style scoped>
    @import '../assets/css/Portfolio.css';
</style>