<template>
    <div :style="{backgroundColor:(isGray) ? '#f1f2f6' : '#ffffff'}" id="contact" class="col-12">
        <h5 :class="(isGray) ? 'title' : 'gray-title'">Contácto</h5>

        <form>
            <div class="form-group">
                <label class="contact-title">Direccion</label>
                <p class="contact-description">Vigo, España</p>
            </div>

            <div class="form-group">
                <label class="contact-title">Numero telefonico</label>
                <p class="contact-description">0412-2106942</p>
            </div>

            <div class="form-group">
                <label class="contact-title">Email</label>
                <p class="contact-description">aragorn.dev0912@gmail.com</p>
            </div>
        </form>

    </div>
</template>

<script>
export default {
    name:'Contact',
    props:['isGray'],
}
</script>

<style scoped>
    @import '../assets/css/Contact.css';
</style>