<template>
    <div class="col-3">
        <div class="card p-2" >
            <img src="../assets/img/17.jpg" class="card-img-top" alt="">
            <div class="card-body">
                <h5 class="little_title">Life Lack Meaning</h5>
                <p class="description">
                    it is a long established fact that a reader will be distracted by readable.
                </p>
                
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'PostsCard',
}
</script>

<style lang="scss" scoped>
.col-3{
    max-width: 340px;
    padding: 0;

    .little_title{
        padding: 10px 0;
    }

    .description{
        line-height: 30px;
        margin:0;
    }
}
</style>