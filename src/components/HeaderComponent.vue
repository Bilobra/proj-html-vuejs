<template>
    <header>
        <nav>
            <ul class="d-flex gap-4 align-items-center link-wrapper">
                <li class="me-auto">
                    <img src="../assets/img/logo-2.png" alt="logo" class="img_logo">
                </li>

                <ProductLinkHeader v-for="(link,i) in LinkArray" :key="i" :link="link.text" :class="link.current? 'border_active' : ''">

                </ProductLinkHeader>

                <li class="p-3 icons_header">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                </li>
                <li class="p-3 icons_header">
                    <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                </li>
                <li>
                    <input type="button" value="Get Started" class="button_default">
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
import ProductLinkHeader from '../components/ProductLinkHeader.vue'
import LinkArray from '../LinkArray'
export default {
    name: 'HeaderComponent',
    components: {
        ProductLinkHeader,
    },
    data() {
        return {
            LinkArray,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

header {
    height: 80px;

    nav {
        max-width: 1154px;
        margin: 0 auto;
        padding: 14px 0;
        // height: 100%;
    }

    .link_wrapper {
        height: 100%;


    }

    .img_logo {
        height: 45px;
        width: auto;
    }

    .icons_header {
        font-size: 12px;
    }

    .border_active, .link_list:hover {
        border-bottom: 2px solid $active-icon-color;
        color : $active-icon-color;
    }
}
</style>