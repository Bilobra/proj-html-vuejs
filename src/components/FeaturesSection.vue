<template>
    <section id="features">
        <div class="row row-cols-1">
            <div class="col-9 d-flex flex-column gap-3 ">
                <h2 class="title ">
                    Popular features that your business needs
                </h2>
                <p class="description">
                    Faff about a quid blower I don't want no agro bleeding chimney <br> pot burke tosser cras nice one boot
                    fanny.!
                </p>
            </div>
            <div class="col-3 d-flex align-items-center">
                <input type="button" value="Explore More Feature" class="button_default button_features">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FeaturesSection',
}
</script>

<style lang="scss" scoped>
#features{
    max-width: 1154px;
    margin: 0 auto 150px;

    .button_features{
        width: 215px;
    }

    .description{
        padding-right: 50px;
    }

    .title{
        margin:0;
    }
}
</style>