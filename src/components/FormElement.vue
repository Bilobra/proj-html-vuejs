<template>
    <div class="form_wrapper row row-cols-1">

        <h4 class="little_title">
            Get in Touch
        </h4>

        <div class="col d-flex gap-4">
            <input type="text" class="form-control bg_form" placeholder="Your name">
            <input type="email" class="form-control bg_form" placeHolder="Your email">
        </div>


        <div class="col-12">
            <input type="text" class="form-control bg_form" placeholder="Your Subject">
        </div>

        <div class="col-12">
            <div class="form-floating">
                <textarea class="form-control bg_form" style="height: 220px">
                </textarea>
                <label for="floatingTextarea2">Your Message</label>
            </div>
        </div>

        <div class="col-12">
            <button type="submit" class=" button_default">Send Message</button>
        </div>

    </div>
</template>

<script>
export default {
    name: 'FormElement',
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

.row {
    gap: 30px;

    .bg_form {
        background-color: #EFF1FE;
        border-color: #00000026;
        font-family: $second-font-family,

    }

    .button_default {
        width: 170px;

    }
    .little_title{
        font-size: 22px;
    }
}
</style>