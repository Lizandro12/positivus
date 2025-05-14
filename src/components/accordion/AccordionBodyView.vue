<template>
    <div class="card_body p-0" :class="{'is_open': props._is_open}">
        <div class="card_body_line"></div>
        <p class="card_text">{{ props._description }}</p>
    </div>
</template>

<script setup>

    const props = defineProps({
        _is_open: {
            type: Boolean,
            required: true
        },
        _description: {
            type: String,
            required: true
        }
    }
    )

</script>

<style scoped>


</style>