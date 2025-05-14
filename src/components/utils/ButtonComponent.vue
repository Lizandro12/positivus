<template>
    <div>
        <button class="btn generic-button">{{ _str }}</button>
    </div>
</template>

<script setup>

const props = defineProps({
    _str: {
        type: String,
        required: true
    }
});

</script>