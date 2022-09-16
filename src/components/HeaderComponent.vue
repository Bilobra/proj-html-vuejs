<template>
    <header>
        <nav>
            <ul class="d-flex gap-4 align-items-center link-wrapper p-0">
                <li class="me-auto">
                    <img src="../assets/img/logo-2.png" alt="logo" class="img_logo">
                </li>

                <ProductLinkHeader v-for="(link,i) in LinkArray" :key="i" :link="link.text"
                    :class="link.current? 'border_active' : ''">

                </ProductLinkHeader>

                <li class="p-2 icons_header">
                    <font-awesome-icon icon="fa-solid fa-magnifying-glass" />

                </li>
                <li class="p-2 icons_header">
                    <font-awesome-icon icon="fa-solid fa-cart-shopping" />
                    <div class="circle_icon">
                        <p class="number_centre">0</p>
                    </div>
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
        font-size: 14px;
        position: relative;

        .circle_icon {
            background-color: #377DFF;
            color: white;
            border-radius: 50%;
            // padding: 2px;
            width: 18px;
            height: 18px;
            aspect-ratio: 1/1;
            vertical-align: middle;
            text-align: center;
            position: absolute;
            top: 0px;
            right: -2px;
            z-index: -1;
            font-size: 10px;

           
        }
    }

    .border_active,
    .link_list:hover {
        border-bottom: 2px solid $active-icon-color;
        color: $active-icon-color;
    }
}
</style>