<template>
    <div  class="col-4 d-flex">
        <div class="marketing_img">
            <img src="../assets/img/24.png" alt="miniLaptop">
        </div>
        <div class="col d-flex flex-column gap-2 ps-3">
            <h3 class="marketing_title">Online Marketing</h3>
            <p class="marketing_description">It is a long established fact that a reader will be distracted</p>
            <ul class="p-0">
                <li v-for="(link,i) in marketingLink" :key="i" class="py-2 mark_link">
                    <span class="marketing_icons">
                        <font-awesome-icon icon="fa-solid fa-check" />
                    </span>
                    {{link.text}}
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MarketingCard',
    data() {
        return {
            marketingLink: [
                {
                    text: 'SEO',
                }, {
                    text: 'SEM',
                }, {
                    text: 'Website Strategy',
                }, {
                    text: 'Social managment',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/VarColor.scss';
    .marketing_title{
        color:$main-text-color;
        font-family : $main-font-family;
        font-size: 22px;
    }
    .marketing_description{
        color:$small-text-color;
        font-family:$second-font-family;
        font-size: 16px;
        line-height: 30px;
    }
    .marketing_img{
        width: 20%;
    }
    .marketing_icons{
        padding-right: 5px;
        color:$active-icon-color;
        font-weight: 600;
    }
    .mark_link{
        font-family: $second-font-family;
        color:$main-text-color;
        font-size: 1rem;
        font-weight: 600;
    }
</style>