<template>
    <div class="col-es-12 task">
        <div class="task-container" data-toggle="modal" :data-target="'#modal_'+id">
            <h5 class="task-title">{{title}}</h5>
            <p class="task-description">{{subtitle}}</p>
        </div>
        
        <Modal :id="id" :images="images" :nameId="'modal_'+id" :title="title" :description="description" :uri="uri" />
    </div>
</template>

<script>

import Modal from './Modal.vue'

export default {
    name:'Task',
    props:['id', 'title', 'subtitle', 'description', 'uri', 'images'],
    components:{
        Modal
    },
}
</script>

<style scoped>
    /*<img class="img-fluid" src="../assets/images/lenna.jpg" alt="alt-img"/>*/
    /*<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModalCenter">
    Launch demo modal
    </button>*/
    @import '../assets/css/Task.css';
</style>