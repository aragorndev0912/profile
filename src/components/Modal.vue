<template>
    <!-- Modal -->
    <div class="modal fade" :id="nameId" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
    <div class="modal-dialog modal-lg" role="document">
        <div class="modal-content">
        <div class="modal-header">
            <!--<h5 class="modal-title" id="modal_title" >{{title}}</h5> -->
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
                        <ol class="carousel-indicators" v-if="images.length > 1">
                            <li v-for="(image, index) in images" v-bind:key="index" :data-target="'#c-indicators'+id" :data-slide-to="index" :class="(index == 0) ? 'active' :''"></li>
                        </ol>
                        <div class="carousel-inner">
                            <div v-for="(image, index) in images" :key="index" :class="(index == 0)? 'carousel-item active': 'carousel-item'">
                                <img class="d-block w-100" :src="getImgUrl(image)" :alt="image">
                            </div>
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
                        <h4 class="mo-title">{{title}}</h4><br/>


                        <p class="mo-text" v-html="description"></p>

                        <br/>
                        <div v-for="(link, index) in uri" v-bind:key="index">
                            <span class="mo-span">- </span> <a class="mo-a" :href="link.uri" target="_blank">{{link.title}}</a>
                        </div>
                    
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
    methods: {
        getImgUrl(pic) {
            return require('../assets/'+pic);
        }
    },
}
</script>

<style scoped>
    @import '../assets/css/Modal.css';
</style>