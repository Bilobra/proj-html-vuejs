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
        <TestimonialSection />
        <PostsSection />
    </main>
</template>

<script>
import HeroSection from './HeroSection.vue'
import MarketingSection from './MarketingSection.vue'
import TrickSection from './TrickSection.vue'
import FeaturesSection from './FeaturesSection.vue'
import TestimonialSection from './TestimonialSection.vue'
import PostsSection from './PostsSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection,
        MarketingSection,
        TrickSection,
        FeaturesSection,
        TestimonialSection,
        PostsSection,
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