<template>
    <div>
        <div :class="`card p-4 card_${props._info.id}`">
            <div class="card-body d-flex flex-column">
                <div class="row h-100 position-relative">
                    <div class="col-6 d-flex flex-column justify-content-between">
                        <h5 class="card_services_title d-flex flex-column align-items-start position-absolute top-0">
                            <span :class="`card_title-${props._info.id} rounded`">{{ props._info.title }}</span>
                            <span :class="`card_title-${props._info.id} rounded`">{{ props._info.subtitle }}</span>
                        </h5>
                        <div class="position-absolute bottom-0">
                            <a href="#" class="card-btn"><img :src="props._info.icon" alt="Icone ver mais"></a>
                            <span :class="`card-read-more card-read-more_${props._info.id} mx-2 d-none d-sm-inline`">Ver mais</span>
                        </div>
                    </div>
                    <div class="col-6 d-flex justify-content-center align-items-end align-items-sm-center">
                        <img class="img-fluid" :src="`/img/card_img_${props._info.id}.png`" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>


const props = defineProps({
    _info: {
        type: Array,
        required: true
    }
})


</script>

<style scoped>

.card {
    border-color: #191A23;
    box-shadow: 5px 5px 0px 0px #191A23;
    border-radius: 2.5rem;
    height: 310px;
}

</style>