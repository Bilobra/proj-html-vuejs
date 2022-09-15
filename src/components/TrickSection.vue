<template>
    <section id="tricks">
        <div class="row row-cols-1">
            <div class="col col-6">
                <h2 class="trick_title">
                    Get tips tricks on how to skyrocket your sales.
                </h2>
                <p class="trick_description">
                    Faff about only a quid blower I don't want no agro bleeding chimrey pot burke tosser cras nice one
                    boot fanny.!
                </p>
                <TrickComponentCard v-for ="(trick,i) in tricks" :key="i" :trickT="trick.title" :trickP="trick.description" :trickImg="trick.img"/>
            </div>
            <div class="col col-6">
                <div class="trick_img">
                    <img src="../assets/img/509.jpeg" alt="GreatIdea">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import TrickComponentCard from './TrickComponentCard.vue'
import tricks from '../TricksArray'
export default {
    name: 'TrickSection',
    components: {
        TrickComponentCard,
    },
    data(){
        return{
            tricks,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

#tricks {
    max-width: 1154px;
    margin: 0 auto 150px;
}
</style>