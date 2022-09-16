<template>
    <div class="col-6">
        <div class="info_wrapper d-flex flex-column gap-3">
            <div>
                <img src="../assets/img/35.png" alt="LogoSoftobox">
            </div>
            <h4 class="little_title">
                9840 Shore St.Fond Du Lac, WI 54935
            </h4>
            <p class="description m-0">
                0 1223 456 789
            </p>
            <p class="description m-0">
                mail@softbox.com
            </p>
        </div>

        <div class="icons_wrapper my-3 d-flex gap-2">
            <font-awesome-icon icon="fa-brands fa-facebook-f" class="icon_form" />
            <font-awesome-icon icon="fa-brands fa-twitter" class="icon_form" />
            <font-awesome-icon icon="fa-brands fa-github" class="icon_form" />
            <font-awesome-icon icon="fa-brands fa-instagram" class="icon_form" />
        </div>

       
            <FormElement/>
       
    </div>
</template>

<script>
    import FormElement from './FormElement.vue'
export default {
    name: 'FormComponent',
    components:{
        FormElement,
    }
}
</script>

<style lang="scss">
.col-6{
    display: flex;
    flex-direction: column;
    gap: 25px;
}
.icons_wrapper{
    .icon_form{
        width: 20px;
        height: 20px;
        // aspect-ratio: 1/1;
        padding: 10px;
        color:#377DFF;
        font-size: 18px;
        border: 1px solid #00000026;
        cursor: pointer;
        
    }
}
</style>