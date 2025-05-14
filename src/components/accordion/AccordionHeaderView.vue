<template>
    <div class="header_card d-flex justify-content-between align-items-center">
        <div class="header_card_info d-flex align-items-center">
            <span class="header_card_number">0{{ props._id }}</span>
            <span class="header_card_title">{{ props._title }}</span>
        </div>
        <div class="d-flex card_icons">
            <div v-if="_is_open" @click="$emit('close_accordion')"><img class="card_icon hide_accordion" src="/img/icon_4.png" alt="Icone esconder accordion"></div>
            <div v-else @click="$emit('open_accordion')"><img class="card_icon show_accordion " src="/img/icon_3.png" alt="Icone abrir accordion"></div>
        </div>
    </div>
</template>

<script setup>

    const props = defineProps({
        _id: {
            type: Number,
            required: true
        },
        _title: { 
            type: String, 
            required: true
        },
        _is_open: {
            type: Boolean, 
            required: true
        }
    }
    ) 
</script>

<style scoped>


</style>