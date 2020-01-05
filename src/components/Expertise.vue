<template>
    <div class="col-12 expertise">
        <h5 class="gray-title">{{title}}</h5>

        <div class="row">
            <div class="col-6">
                <ExpertiseDescription  title="Professionally drive" description="Synergistically strategize customer directed resources rather than principle." />
            </div>
            <div class="col-6">
                <ExpertiseDescription  title="Seamlessly leverage" description="Quickly repurpose reliable customer service with orthogonal ideas. Competently." />
            </div>
            <div class="col-6">
                <ExpertiseDescription  title="Interactively incubate" description="Interactively myocardinate high standards in initiatives rather than next-generation." />
            </div>
            <div class="col-6">
                <ExpertiseDescription  title="Globally streamline" description="Dynamically initiate client-based convergence vis-a-vis performance based." />
            </div>
        
        </div>
    </div>
</template>

<script>

import ExpertiseDescription from './ExpertiseDescription.vue'

export default {
    name:'Expertise',
    props:['title'],
    components:{
        ExpertiseDescription,
    }

}
</script>

<style scoped>
    @import '../assets/css/Expertise.css';
</style>