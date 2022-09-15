<template>
    <section id="posts">
        <div class="content">
            <h2 class="title mb-4">
                Lastest Posts
            </h2>
            <p class="description m-0">
                If you are planning on developing a produc landing
            </p>
        </div>
        <div class="row row-cols-1 justify-content-between">
            <PostsCard v-for="(card,i) in CardImage" :key="i" :image="card.image" />

        </div>
    </section>
</template>

<script>
import PostsCard from './PostsCard.vue'
export default {
    name: 'PostsSection',
    components: {
        PostsCard,
    },
    data() {
        return {
            CardImage: [
                {
                    image: require('../assets/img/18.jpg'),
                },
                {
                    image: require('../assets/img/19.jpg'),
                },
                {
                    image: require('../assets/img/20.jpg'),
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
#posts {
    background-color: #EFF1FE;
    padding: 110px 0;

    .row {
        max-width: 1154px;
        margin: 0 auto;
        padding: 110px 0;

    }
}
</style>