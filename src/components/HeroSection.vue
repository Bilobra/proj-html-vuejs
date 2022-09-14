<template>
    <div class="row row-cols-1">
        <div class="col-6 d-flex flex-column gap-4 col_info">
            <h2 class="hero_title">
                The biggest platform for your growth.
            </h2>
            <p class="hero_description">
                There are many variations of passages of Lorem Ipsum avaiable, but the majority have suffred alteration
                in some form
            </p>
            <div class="hero_button">
                <input type="button" value="Read More" class="button_default">

            </div>
        </div>
        <div class="col-6 ">
            <img src="../assets/img/27-1.png" alt="hero-img peopletalking" class="img_h">
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeroSection',
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

.col_info {
    padding-top: 80px;
    padding-right: 110px;
}

.img_h {
    height: 510px;
    position: relative;
    bottom: -40px;
}

.hero_title {
    font-size: 51px;
    font-family: $main-font-family;
}

.hero_description {
    font-size: 16px;
    color: $small-text-color;
    font-family: $second-font-family;
    
}
</style>