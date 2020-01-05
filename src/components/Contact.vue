<template>
    <div id="contact" class="col-12">
        <h5 class="gray-title">Contact</h5>

        <form>
            <div class="form-group">
                <label class="contact-title">Address</label>
                <p class="contact-description">1355 Market Street, Suite 900 <br/>
                    San Francisco, CA 94103</p>
            </div>

            <div class="form-group">
                <label class="contact-title">Phone Number</label>
                <p class="contact-description">+61 3 8376 6284</p>
            </div>

            <div class="form-group">
                <label class="contact-title">Mobile Number</label>
                <p class="contact-description">987 654 321</p>
            </div>

            <div class="form-group">
                <label class="contact-title">Email</label>
                <p class="contact-description">coffee@amelie.me</p>
            </div>
        </form>

    </div>
</template>

<script>
export default {
    name:'Contact',
}
</script>

<style scoped>
    @import '../assets/css/Contact.css';
</style>