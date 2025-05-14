<template>
    <div class="container py-5">
        <div class="d-flex flex-column flex-lg-row align-items-center py-5">
            <h2 class="title rounded me-0 me-sm-5">Serviços</h2>
            <p class="paragraph text-center text-lg-start">Na nossa agência de marketing digital, oferecemos um conjunto de serviços para ajudar negocios a crescerem e terem sucesso online. Estes serviços incluem:</p>
        </div>
        <div class="row g-5 mt-1">
            <div class="col-12 col-lg-6" v-for="info in card_info" :key="info.id">
                <card-component :_info="info"/>
            </div>
        </div>

    </div>
</template>

<script setup>
import CardComponent from '../utils/CardComponent.vue';

const card_info = [
    {
        id: 1,
        title: "SEO",
        subtitle: "",
        icon: "/img/icon_2.png",
        background_class: "card_1"
    },
    {
        id: 2,
        title: "Publicidade",
        subtitle: "paga por clique",
        icon: "/img/icon_2.png",
        background_class: "card_2"

    },
    {
        id: 3,
        title: "Marketing de",
        subtitle: "mídia social",
        icon: "/img/icon_1.png",
    },
    {
        id: 4,
        title: "Email",
        subtitle: "marketing",
        icon: "/img/icon_2.png",
    },
    {
        id: 5,
        title: "Criação de",
        subtitle: "Conteúdo",
        icon: "/img/icon_2.png",
    },
    {
        id: 6,
        title: "Análise e",
        subtitle: "rastreamento",
        icon: "/img/icon_1.png",
    }
]

</script>

<style scoped>

</style>