<template>
    <main>
        <section id="hero_section">
            .<div class="container_hero_section">
                <HeroSection />
            </div>
        </section>
        <MarketingSection />
    </main>
</template>

<script>
import HeroSection from './HeroSection.vue'
import MarketingSection from './MarketingSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection,
        MarketingSection,
    }
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

#hero_section {
    background-color: $jumbo-bg-color;
    margin-bottom: 150px;

    .container_hero_section {
        max-width: 1441px;
        margin: 0 auto;
    }
}
</style>