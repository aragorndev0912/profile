<template>
    <!-- Modal -->
    <div class="modal fade" :id="nameId" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
    <div class="modal-dialog modal-dialog-centered" role="document">
        <div class="modal-content">
        <div class="modal-header">
            <h5 class="modal-title" id="modal_title" >{{title}}</h5>
            <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
            </button>
        </div>
        <div class="modal-body">
            <div class="container-fluid">
                <div class="row">
                    {{description}}
                </div>
            </div>
        </div>
        <!--<div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
        </div>-->
        </div>
    </div>
    </div>
</template>

<script>
export default {
    name:'Modal',
    props:['nameId', 'title', 'description'],
    
    
}
</script>

<style scoped>
    @import '../assets/css/Modal.css';
</style>