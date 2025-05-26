<template>
    <div class="card use_cases_card ">
        <div class="card-body">
            <p class="card-text cases_card_text">{{ props._cas.text }}</p>
            <a href="#" class="card-link d-flex card_link_text">Ler mais <icon-arrow-up-right class="ms-2"/></a>
        </div>
    </div>
</template>

<script setup>
import IconArrowUpRight from '../icons/IconArrowUpRight.vue';

const props = defineProps({
    _cas: {
        type:Object,
        required: true
    }
})
</script>