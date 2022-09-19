<template>
    <main>
        <section id="hero_section">
            <div class="container_hero_section">
                <HeroSection />
            </div>
        </section>
        <MarketingSection />
        <TrickSection />
        <FeaturesSection />
        <TestimonialSection />
        <PostsSection />
        <ContactsSection />
    </main>
</template>

<script>
import HeroSection from './HeroSection.vue'
import MarketingSection from './MarketingSection.vue'
import TrickSection from './TrickSection.vue'
import FeaturesSection from './FeaturesSection.vue'
import TestimonialSection from './TestimonialSection.vue'
import PostsSection from './PostsSection.vue'
import ContactsSection from './ContactsSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection,
        MarketingSection,
        TrickSection,
        FeaturesSection,
        TestimonialSection,
        PostsSection,
        ContactsSection,
    }
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

#hero_section {
    background-color: $jumbo-bg-color;
    margin: 0 auto 150px;
    max-width: 1441px;

    .container_hero_section {
        max-width: 1360px;
        margin: 0 auto;
    }
}
</style>