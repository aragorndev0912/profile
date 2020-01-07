<template>
    <!-- Modal -->
    <div class="modal fade" :id="nameId" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
    <div class="modal-dialog modal-lg" role="document">
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
                    <div class="col-12">
                    <!---->
                    <div :id="'c-indicators'+id" class="carousel slide" data-ride="carousel">
                        <ol class="carousel-indicators">
                            <li :data-target="'#c-indicators'+id" data-slide-to="0" class="active"></li>
                            <li :data-target="'#c-indicators'+id" data-slide-to="1"></li>
                        </ol>
                        <div class="carousel-inner">
                            <div v-for="(image, index) in images" :key="index" :class="(index == 0)? 'carousel-item active': 'carousel-item'">
                                <img class="d-block w-100" src="../assets/images/girl.jpg" :alt="image">
                            </div>

                            <!--<div class="carousel-item active">
                            <img class="img-fluid d-block w-100" src="../assets/images/girl.jpg" alt="First slide">
                            </div>
                            <div class="carousel-item">
                            <img class="img-fluid d-block w-100" src="../assets/images/girl.jpg" alt="Second slide">
                            </div>
                            <div class="carousel-item">
                            <img class="img-fluid d-block w-100" src="../assets/images/girl.jpg" alt="Third slide">
                            </div>-->
                        </div>
                        <!--<a class="carousel-control-prev" href="#c-indicators" role="button" data-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="sr-only">Previous</span>
                        </a>
                        <a class="carousel-control-next" href="#c-indicators" role="button" data-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="sr-only">Next</span>
                        </a>-->
                    </div>
                    <!---->
                    </div>
                    <div class="container-blank col-12">
                        <h4>{{title}}</h4><br/>


                        <p class="mo-text" v-html="description"></p>

                        <br/>
                        <span class="mo-span">Link: </span> <a class="mo-a" :href="uri" target="_blank">{{uri}}</a>
                    </div>
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
    props:['id', 'nameId', 'title', 'description', 'uri', 'images'],
    
    
}
</script>

<style scoped>
    @import '../assets/css/Modal.css';
</style>