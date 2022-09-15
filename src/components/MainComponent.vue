<template>
    <main>
        <section id="hero_section">
            .<div class="container_hero_section">
                <HeroSection />
            </div>
        </section>
        <MarketingSection />
        <TrickSection />
        <FeaturesSection />
    </main>
</template>

<script>
import HeroSection from './HeroSection.vue'
import MarketingSection from './MarketingSection.vue'
import TrickSection from './TrickSection.vue'
import FeaturesSection from './FeaturesSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection,
        MarketingSection,
        TrickSection,
        FeaturesSection,
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