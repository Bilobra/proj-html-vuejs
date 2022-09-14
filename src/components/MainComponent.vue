<template>
    <main>
        <section id="hero_section">
            .<div class="container_hero_section">
                <HeroSection />

            </div>
        </section>
    </main>
</template>

<script>
import HeroSection from './HeroSection.vue'
export default {
    name: 'MainComponent',
    components: {
        HeroSection,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/VarColor.scss';
    #hero_section{
        background-color: $jumbo-bg-color;

        .container_hero_section{
            max-width: 1441px;
            margin: 0 auto;
        }
    }
</style>