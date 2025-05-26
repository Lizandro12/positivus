<template>
    <div class="container py-5">
        <div class="d-flex flex-column flex-lg-row align-items-center">
            <h3 class="how-it-works-accordion-title me-0 me-md-5 ">Como funciona</h3>
            <p class="how-it-works-accordion-paragraph">Guia passo a passo para atingir seus objetivos de negócios</p>
        </div>
        <div class="row cards">
            <div class="col-12 mt-4 mb-sm-0">
                <div class="card" :class="{'background': info.is_open}" v-for="info in accordion_info" :key="info.id">
                    <accordion-header-view
                        :_id="info.id"
                        :_title="info.title"
                        :_is_open="info.is_open"
                        @open_accordion="toggleAccordion(info)"
                        @close_accordion="toggleAccordion(info)"
                    />
                    <accordion-body-view
                    :_is_open="info.is_open"
                    :_description="info.description"
                    />
                </div>
            </div>
        </div>
    </div>
    
</template>


<script setup>
import AccordionHeaderView from './AccordionHeaderView.vue';
import AccordionBodyView from './AccordionBodyView.vue';
import { reactive } from 'vue';


const accordion_info = reactive( [
    {
        id: 1,
        title: 'Consultoria',
        description: 'Durante a consulta inicial, discutiremos suas metas e objetivos de negócios, seu público-alvo e suas iniciativas de marketing atuais. Isso nos permitirá entender suas necessidades e adaptar nossos serviços às suas necessidades.',
        is_open: false
    },
    {
        id: 2,
        title: 'Pesquisa e Desenvolvimento de Estratégia',
        description: 'Realizamos uma análise detalhada do mercado, público-alvo e concorrência. A partir disso, desenvolvemos estratégias personalizadas e orientadas por dados. Nosso objetivo é gerar resultados reais e fortalecer sua marca.',
        is_open: false
    },
    {
        id: 3,
        title: 'Implementação',
        description: 'Colocamos a estratégia em prática com precisão e criatividade. Executamos campanhas, conteúdos e ações em múltiplos canais Tudo é monitorado de perto para garantir performance e ajustes ágeis.',
        is_open: false
    },
    {
        id: 4,
        title: 'Optimização e Monitoramento',
        description: 'Acompanhamos continuamente os resultados de cada ação. Analisamos métricas-chave para identificar oportunidades de melhoria. Otimizamos as campanhas em tempo real para máxima eficiência.',
        is_open: false
    },
    {
        id: 5,
        title: 'Relatórios e Comunicação',
        description: 'Enviamos relatórios claros com dados e insights sobre os resultados. Mantemos uma comunicação transparente e contínua com o cliente. Você acompanha cada etapa e evolução das campanhas com clareza.',
        is_open: false
    },
    {
        id: 6,
        title: 'Melhoria Contínua',
        description: 'Avaliamos constantemente os resultados para identificar novas oportunidades. Ajustamos estratégias com base em dados e feedbacks. Nosso foco é evoluir sempre, buscando melhores resultados a cada ciclo.',
        is_open: false
    }
]
)

const toggleAccordion = (info) => {
    accordion_info.forEach(obj => {
        obj.is_open == true ?  obj.is_open = false : obj.is_open = obj.id === info.id;
    });

}



</script>


<style scoped>

.card {
    border-color: #191A23;
    border-radius: 45px;
    padding: 2rem 2rem;
    box-shadow: 5px 5px 0px 0px #191A23;
    margin-bottom: 1rem;
    transition: .3s ease all;
}

.card.background {
    background-color: #B9FF66;
}

@media (max-width:576px) {
    .how-it-works-accordion-title {
        max-width: 250px;
    } 

    .card {
        padding: 1.4rem 1.5rem;
    }
}
</style>