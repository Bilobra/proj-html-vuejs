<template>

    <div class="features_wrapper">

        <div class="bg_circle">
            
        </div>

        <section id="features">

            <div class="row row-cols-1">
                <div class="col-9 d-flex flex-column gap-3 ">
                    <h2 class="title ">
                        Popular features that your business needs
                    </h2>
                    <p class="description">
                        Faff about a quid blower I don't want no agro bleeding chimney <br> pot burke tosser cras nice
                        one
                        boot
                        fanny.!
                    </p>
                </div>
                <div class="col-3 d-flex align-items-center justify-content-end pe-4">
                    <input type="button" value="Explore More Feature" class="button_default button_features">
                </div>
            </div>

            <div class="row row-cols-1 gap-4 justify-content-between">
                <FeaturesCard v-for="(el,i) in grid" :key="i" :el="el" :class="el.bg? el.bg : '' " />

            </div>
        </section>
    </div>
</template>

<script>
import FeaturesCard from './FeaturesCard.vue'
import grid from '../GridArray'
export default {
    name: 'FeaturesSection',
    components: {
        FeaturesCard,
    },
    data() {
        return {
            grid,
        }
    },
}
</script>

<style lang="scss" scoped>
    .features_wrapper{
        position:relative;
    }
.bg_circle {
    background-image: url('../assets/img/14.png');
    background-repeat: no-repeat;
    min-height: 100%;
    width: 100%;
    position: absolute;
    left: -595px;
    bottom: 70px;
    // background-position: left;
    z-index:-1;
}

#features {
    max-width: 1154px;
    margin: 0 auto 150px;


    .button_features {
        width: 215px;
    }

    .description {
        padding-right: 50px;
    }

    .title {
        margin: 0;
    }

    .row {

        .green_bg:hover {
            background-color: #6CDAC1;
            color: white !important;
        }

        .blu_bg:hover {
            background-color: #377DFF;
            color: white !important;

        }

        .salmon_bg:hover {
            background-color: #FF796D;
            color: white !important;

        }


    }
}
</style>