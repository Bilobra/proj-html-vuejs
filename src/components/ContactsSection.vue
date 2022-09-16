<template>
    <section id="contacts">
        <div class="content">
            <h2 class="title mb-4">
                Contacts with our team
            </h2>
            <p class="description m-0">
                If you are planning on developing a produc landing
            </p>
        </div>
        <div class="row row-cols-1">
           
                <MapComponent/>
           
        </div>
    </section>
</template>

<script>
import MapComponent from './MapComponent.vue'
export default {
    name: 'ContactsSection',
    components: {
        MapComponent,
    }
}
</script>

<style lang="scss" scoped>
#contacts {
    background-color: #EFF1FE;
    padding: 110px 0;
}

.row{
    max-width: 1154px;
    margin: 0 auto;
}
.content{
    margin-bottom: 110px;
}
</style>