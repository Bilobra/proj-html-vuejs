<template>
    <section id="posts">
        <div class="content">
            <h2 class="title mb-4">
                Lastest Posts
            </h2>
            <p class="description">
                If you are planning on developing a produc landing
            </p>
        </div>
        <div class="row row-cols-1 justify-content-between">
            <PostsCard v-for="n in 3" :key="n" />

        </div>
    </section>
</template>

<script>
import PostsCard from './PostsCard.vue'
export default {
    name: 'PostsSection',
    components: {
        PostsCard,
    }
}
</script>

<style lang="scss" scoped>
#posts {
    background-color: #EFF1FE;
    padding: 110px 0;

    .row {
        max-width: 1154px;
        margin:0 auto;

    }
}
</style>