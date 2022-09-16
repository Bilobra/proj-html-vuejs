<template>
    <div class="col-3">
        <div class="card p-2" >
            <img :src="image" class="card-img-top" alt="">
            <div class="card-body">
                <h5 class="little_title">Life Lack Meaning</h5>
                <p class="description">
                    it is a long established fact that a reader will be distracted by readable.
                </p>
                
            </div>
            <div class="badge_date description m-0">
                November 28,2019
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'PostsCard',
    props:{
        image:String,
    }
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
    .card{
        position: relative;
    }
    .badge_date{
        padding: 3px 8px;
        line-height: 20px;
        position: absolute;
        background-color: white;
        border-radius: 3px;
        top: 15px;
        left:15px;
        font-size: 12px;
    }
}
</style>