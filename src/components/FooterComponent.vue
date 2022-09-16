<template>
    <section id="footer_section">
        <div class="row row-cols-1 row_footer">
            <div class="col-6 col_logo">
                <div>
                    <img src="../assets/img/35.png" alt="logoSoftbox">

                </div>
                <p class="description">
                    It is a long established fact that a reader will be distracted by the readable content.
                </p>
                <p class="description">Copyright @ 2018 <span class="blue_text">Softbox</span></p>
            </div>



            <FooterElementLink />




        </div>
    </section>
</template>

<script>
import FooterElementLink from './FooterElementLink.vue'
export default {
    name: 'FooterComponent',
    components: {
        FooterElementLink,
    },

}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

#footer_section {
    background-color: #EFF1FE;
    border-top: 1px solid #00000026;
    
}

.row_footer {
    max-width: 1154px;
    margin: 0 auto;
    padding: 80px 0;

    .col_logo {
        padding-right: 180px;
    }
}

.blue_text {
    color: #377DFF
}
</style>