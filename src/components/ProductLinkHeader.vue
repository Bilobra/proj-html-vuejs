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
    padding: 8px 10px;
    line-height: 45px;
    font-size: 14px;
    color:$main-text-color;
}
</style>