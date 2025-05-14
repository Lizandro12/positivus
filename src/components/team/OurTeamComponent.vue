<template>
    <div class="container mb-5">
        <div class="d-flex flex-column flex-lg-row align-items-center pt-5">
            <h2 class="title rounded me-0 me-sm-5">Nossa Equipe</h2>
            <p class="paragraph text-center text-lg-start">Conheça a equipe qualificada e experiente por trás de nossas estratégias de marketing digital de sucesso</p>
        </div>
        <div class="row g-4 g-sm-3 g-lg-4 mt-5">
            <div v-for="member in team_members" :key="member.id" class="col-12 col-sm-6 col-lg-4">
                <team-card-component :_member="member"/>
            </div>
        </div>
        <div class="text-end py-4">
            <button-component :_str="message"/>
        </div>
    </div>
</template>

<script setup>
import TeamCardComponent from './TeamCardComponent.vue';
import ButtonComponent from '../utils/ButtonComponent.vue';

const message = "Ver toda a equipe"

const team_members = [
    {
        id: 1,
        name: "John Smith",
        position: "CEO e Fundador",
        description:
        "Mais de 10 anos de experiência em marketing digital. Expertise em SEO, PPC e estratégia de conteúdo.",
        image: "/img/picture_1.png",
        linkedin: "#",
    },
    {
        id: 2,
        name: "Janie Doe",
        position: "Directora de Operações",
        description:
        "Mais de 7 anos de experiência em gestão de projetos e liderança de equipes. Fortes habilidades de organização e comunicação.",
        image: "/img/picture_2.png",
        linkedin: "#",
    },
    {
        id: 3,
        name: "Michael Brown",
        position: "Especialista SEO Senior",
        description:
        "Mais de 5 anos de experiência em SEO e criação de conteúdo. Proficiência em pesquisa de palavras-chave e otimização on-page.",
        image: "/img/picture_3.png",
        linkedin: "#",
    },
    {
        id: 4,
        name: "Emily Johnson",
        position: "Gestora PPC",
        description:
        "Mais de 3 anos de experiência em publicidade de pesquisa paga. Habilidade em gestão de campanhas e análise de desempenho.",
        image: "/img/picture_4.png",
        linkedin: "#",
    },
    {
        id: 5,
        name: "Brian Williams",
        position: "Especialista em Mídias Sociais",
        description:
        "Mais de 4 anos de experiência em marketing de mídias sociais. Proficiente na criação de conteúdo envolvente, análise de métricas e construção de engajamento.",
        image: "/img/picture_5.png",
        linkedin: "#",
    },
    {
        id: 6,
        name: "Sarah Kim",
        position: "Cradora de Conteúdos",
        description:
        "Mais de 2 anos de experiência em redação e edição. Habilidade na criação de conteúdo envolvente e otimizado para SEO para diversos setores.",
        image: "/img/picture_6.png",
        linkedin: "#",
    },
]

</script>