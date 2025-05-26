<template>
    <div class="container py-5">
        <div class="d-flex flex-column flex-lg-row align-items-center pt-5 pb-5">
            <h2 class="title rounded me-0 me-sm-5 cases_studies_title">Casos de Estudo</h2>
            <p class="paragraph text-center text-lg-start">Explore exemplos reais do nosso sucesso comprovado no Marketing Digital através dos nossos Casos de Estudo</p>
        </div>
        <div class="cases_swipper_container py-4 mt-1">
                    <swiper-container
        :pagination="false"
        :loop="true"
        :autoplay-delay="2500"
        :autoplay-disable-on-interaction="false"
        :breakpoints= "{
            576: {
              slidesPerView: 1.2,
              spaceBetween: 20
              },
            640: {
              slidesPerView: 1.2,
              spaceBetween: 20
            },
            768: {
              slidesPerView: 1.2,
              spaceBetween: 30
            },
            992: {
              slidesPerView: 3,
            },
            1200: {
              slidesPerView: 3,
            }
            }">
            <swiper-slide v-for="cas in cases" :key="cas.id" >
                <cases-studies-card-component :_cas="cas" />
            </swiper-slide>
        </swiper-container>
        </div>

    </div>
</template>

<script setup>
import CasesStudiesCardComponent from '../utils/CasesStudiesCardComponent.vue';

const cases = [
    {
        id: 1,
        text: "Para um restaurante local, implementamos uma campanha PPC direcionada que resultou em um aumento de 50% no tráfego do site e um aumento de 25% nas vendas.",
    },
    {
        id: 2,
        text: "Para uma empresa de software B2B, desenvolvemos uma estratégia de SEO que resultou em uma classificação alta e um aumento de 200% no tráfego orgânico.",
    },
    {
        id: 3,
        text: "Para uma rede nacional de varejo, criamos uma campanha de marketing de mídia social que aumentou os seguidores em 25% e gerou um aumento de 20% nas vendas online.",
    }
]

</script>

<style scoped>

swiper-container {
    width: 100%;
  }

swiper-slide {
    font-size: 18px;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>