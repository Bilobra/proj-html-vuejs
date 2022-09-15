<template>
    <div class="col m-0" :class="el.bg">
        <h4 class="little_title">{{el.title}}</h4>
        <figure class="m-0">
            <img :src="el.img" :alt="el.title">
        </figure>
    </div>
</template>

<script>
export default {
    name: 'FeaturesCard',
    props: {
        el: Object,
    }
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

.col {
    width: 236px;
    padding: 25px 0px 30px 15px;
    box-shadow: 0px 4px 20px #0000001f;

    transition: all 300ms;


    .little_title {
        font-family: $main-font-family;
        // color: #1E1E1E;
        font-size: 20px;
    }
}
</style>