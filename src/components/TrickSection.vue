<template>
    <section id="tricks">
        <div class="row row-cols-1">
            <div class="col col-6">
                <h2 class="title">
                    Get tips tricks on how to skyrocket your sales.
                </h2>
                <p class="description">
                    Faff about only a quid blower I don't want no agro bleeding chimrey pot burke tosser cras nice one
                    boot fanny.!
                </p>
                <TrickComponentCard v-for="(trick,i) in tricks" :key="i" :trick="trick"
                    :class="trick.current? 'active_card' : ''" />
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
    data() {
        return {
            tricks,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/VarColor.scss';

#tricks {
    max-width: 1154px;
    margin: 0 auto 120px;
}



.active_card {

    box-shadow: 0px 40px 20px rgb(0 0 0 / 19%);
}
</style>