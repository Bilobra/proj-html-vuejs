<template>
    <div class="col d-flex flex-column">
        <div>
            <img :src="trickImg" alt="">
        </div>
        <div>
            <h2>{{trickT}}</h2>
            <p>{{trickP}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TrickComponentCard',
    props: {
        trickT: String,
        trickImg: String,
        trickP :String,
    }

}
</script>

<style lang="scss" scoped>

</style>