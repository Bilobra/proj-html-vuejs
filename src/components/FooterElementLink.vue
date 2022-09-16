<template>
    <div class="col-6 d-flex flex-column">
        <div class="row row-cols-1 justify-content-between">
            <ul class="col-3 p-0" v-for="(link,i) in footerLink" :key="i">
                <h4 class="little_title">{{link.title}}</h4>
                <li v-for="(link,i) in footerLink" :key="i" class="description m-0 py-4">{{link.link[i]}}</li>

            </ul>

        </div>

    </div>
</template>

<script>
import footerLink from '../FooterLinkArray'
export default {

    name: 'FooterElementLink',
    data() {
        return {
            footerLink,
        }
    }


}
</script>

<style lang="scss">

</style>