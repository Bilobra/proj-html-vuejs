<template>
    <li class="link_list">
        <a href="#">
            {{link}}
        </a>
    </li>
</template>

<script>
export default {
    name: 'ProductLinkHeader',
    props: {
        link: String,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/VarColor.scss';
.link_list {
    align-self: flex-end;
    padding-bottom: 12px ;
    // line-height: 45px;
    font-size: 14px;
    color:$main-text-color;
    font-family: $second-font-family;
}
</style>