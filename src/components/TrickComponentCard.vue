<template>
    <div class="col d-flex pt-5">
        <div class="img_trick">
            <img :src="trick.img" alt="">
        </div>
        <div>
            <h2 class="title" :class="trick.current? 'active_title' : ''">{{trick.title}}</h2>
            <p class="description">{{trick.description}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TrickComponentCard',
    props: {
        trick: Object,
    }

}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

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

.img_trick {
    width: 45%;
    padding: 20px 10px;
}
.active_title{
    color:$active-icon-color;
}

</style>