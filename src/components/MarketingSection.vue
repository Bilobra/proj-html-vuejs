<template>
    <section id="marketing">
        <div class="row row-cols-1">
            <MarketingCard v-for="n in 3" :key="n"/>
        </div>

    </section>
</template>

<script>
import MarketingCard from './MarketingCard.vue'
export default {
    name: 'MarketingSection',
    components: {
        MarketingCard,
    }
}
</script>

<style lang="scss" scoped>
#marketing {
    max-width: 1154px;
    margin: 0 auto 150px;
}
</style>