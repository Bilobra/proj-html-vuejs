<template>
    <section id="testimonials">
        <div class="wrap_testimonials d-flex align-items-center">
            <div class="content">
                <h2 class="title mb-4">
                    Our Testimonials
                </h2>
                <p class="description">
                    If you are planning on developing a produc landing app or website, take a look at this
                    beautiful-crafted
                </p>
            </div>
        </div>
        <div class="card_container">
            <div class="row row-cols-1 gap-3 d-flex justify-content-center">
                <div class=" col_card col-6">
                    <figure class="img_testimonial">
                        <img src="../assets/img/26.jpeg" alt="">
                    </figure>
                    <div>
                        <span class="title">Juli Aaan</span>
                        <span class="description">- COO Softbox</span>
                    </div>
                    <p class="description">
                        At vero eos et accusamus et iusto odio dignissimos dicusimus qui blanditiis prasentium vero eos
                        et consectetur accus adip adip.
                    </p>

                </div>
                <div class=" col_card col-6">
                    <figure class="img_testimonial">
                        <img src="../assets/img/27.jpeg" alt="">
                    </figure>
                    <div>
                        <span class="title">Mac Znder</span>
                        <span class="description">- Manager Softbox</span>
                    </div>
                    <p class="description">
                        At vero eos et accusamus et iusto odio dignissimos dicusimus qui blanditiis prasentium vero eos
                        et consectetur accus adip adip.
                    </p>

                </div>


                <div class="d-flex justify-content-center gap-3 align-items-center pb-3">
                    <div class="dot_slide active">

                    </div>
                    <div class="dot_slide">

                    </div>
                </div>


            </div>
        </div>

    </section>
</template>

<script>
export default {
    name: 'TestimonialSection',
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

#testimonials {
    background-color: #EFF1FE;
}

.wrap_testimonials {
    background-image: url('../assets/img/15.png');
    background-color: #EFF1FE;
    min-height: 310px;
    background-repeat: no-repeat;
}



.card_container {
    max-width: 1154px;
    margin: 0 auto;
    padding-top: 20px;



    .col_card {
        display: flex;
        flex-direction: column;
        max-width: 500px;

        align-items: center;
        padding: 50px 30px;
        gap: 40px;
        box-shadow: 0px 4px 20px #0000001f;
        margin-bottom: 50px;
        background-color: #FFFFFF;



        img {
            width: 65px;
            height: 65px;
            aspect-ratio: 1/1;
            border-radius: 50%;

        }

        .title {
            font-family: $main-font-family;
            color: $main-text-color;
            font-size: 25px;
        }

        .description {
            font-family: $second-font-family;
            color: $small-text-color;
            font-size: 16px;
            line-height: 30px;
        }
    }

    .dot_slide {
        height: 15px;
        width: 15px;
        border: 1px solid #1E1E1E;
        border-radius: 50%;
        background-color: #1E1E1E;

        &.active {
            background-color: #377DFF;
            border-color: #377DFF;
        }
    }
}
</style>