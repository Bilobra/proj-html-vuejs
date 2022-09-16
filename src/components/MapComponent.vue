<template>
    <div class="col-6">
        <img src="../assets/img/StaticMapService.GetMapIma.png" alt="mapImg">

        <div class=" indications_wrapper d-flex gap-4">
            <div>
                <h5 class="little_title">Storey Ave</h5>
                <p class="description mb-3">San Francisco, California 94129</p>
                <p class="description  blue_link m-0">Visualizza mappa più grande</p>
            </div>
            <div class="text-center">
                <font-awesome-icon icon="fa-solid fa-turn-up" class="blue_link fs_icon" />
                <p class="description blue_link m-0">Indicazioni</p>
            </div>

        </div>
        <div class="zoom_wrapper d-flex flex-column">
            <font-awesome-icon icon="fa-solid fa-plus" class="zoom_icons zoom_plus" />
            <font-awesome-icon icon="fa-solid fa-minus" class="zoom_icons" />
        </div>
    </div>
</template>

<script>
export default {
    name: 'MapComponent',
}
</script>

<style lang="scss" scoped>
.col-6 {
    position: relative;
}

.indications_wrapper {
    // max-width: 100px;
    padding: 15px 10px;
    position: absolute;
    top: 10px;
    left: 25px;
    background-color: white;
    border-radius: 3px;
    box-shadow: 2px 1px 6px #8080808c;
}

.description {
    font-size: 14px;
}

.blue_link {
    color: #377DFF
}

.fs_icon {
    font-size: 30px;
    margin-bottom: 10px;
}

.little_title {
    font-weight: 600;
}

.zoom_wrapper {
    position: absolute;
    // bottom: 10px;
    top: 320px;
    right: 25px;
    background-color: white;
    padding: 5px;
    border-radius: 2px;
    box-shadow: 2px 1px 6px #8080808c;


    .zoom_plus {
        border-bottom: 1px solid #00000026;
    }

    .zoom_icons {
        font-size: 20px;
        padding: 12px;
        color: #495057 // font-weight: 600;
    }

}
</style>