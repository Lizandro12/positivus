<template>
    <div class="card h-100 text-center py-5 px-4 shadow-sm team_card">
        <div class="d-flex align-items-end pb-2 border-bottom">
            <div class="me-4">
                <img :src="props._member.image" class="img-fluid" width="80" height="80" alt="Photo" />
            </div>
            <div class="text-start">
                <h5 class="mb-1">{{ props._member.name }}</h5>
                <p class="text-muted mb-1">{{ props._member.position }}</p>
            </div>
        </div>
        <p class="small text-start mt-3">{{ props._member.description }}</p>
        <a :href="props._member.linkedin" target="_blank" class="text-dark">
            <img src="/img/linkedin.png" alt="LinkedIn" class="linkedin_icon">
        </a>
    </div>
</template>

<script setup>

const props = defineProps({
    _member: {
        type: Object,
        required: true
    }
})
</script>

<style scoped>

.team_card {
  border-radius: 2.5rem !important;
  border: #191A23 1px solid;
  box-shadow: 5px 5px 0px 0px #191A23 !important;
  position: relative;
}

.text-dark {
    position: absolute;
    right: 30px;
    top: 30px;
}




img {
  object-fit: cover;
}
</style>
