<template>
  <div class="container position-relative">
    <div class="d-flex flex-column flex-lg-row align-items-center pt-4 pb-5">
        <h2 class="title rounded me-0 me-sm-5">Testemunhos</h2>
        <p class="paragraph text-center text-lg-start">Ouça dos nossos clientes satisfeitos: Leia nossos testemunhos para saber mais sobre nossos serviços de Marketing Digital.</p>
    </div>
    <div class="testimonial py-5 my-4 ">
      <swiper-container
        navigation-prev-el=".swiper-button-custom-prev"
        navigation-next-el=".swiper-button-custom-next"
        :autoplay-delay="2500"
        :autoplay-disable-on-interaction="false"
        :space-between="50"
        :navigation="true"
        :pagination="true"
        :loop="true"
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
                slidesPerView: 2.5,
              },
              1200: {
                slidesPerView: 2.5,
              }
              }"
      >
      <swiper-slide v-for="testimonial in testimonials" :key="testimonial.id">
          <div class="card text-white p-4 h-100">
              <p class="fs-6 fst-italic">"{{ testimonial.text }}"</p>
              <div class="mt-4">
          </div>
          </div>
          <p class="fw-bold text-white text-center text-sm-start ms-0 ms-sm-5 mb-0 mt-5">{{ testimonial.name }}</p>
          <p class="text-white text-center text-sm-start ms-0 ms-sm-5" ><small>{{ testimonial.position }}</small></p>
      </swiper-slide>
      </swiper-container>
      <div class="swiper-button-custom-prev">
        <icon-arrow-left/>
      </div>
      <div class="swiper-button-custom-next">
        <icon-arrow-right/>
      </div>
    </div>
  </div>
</template>

<script setup>

import IconArrowLeft from '../icons/IconArrowLeft.vue';
import IconArrowRight from '../icons/IconArrowRight.vue';


const testimonials =  [
        {
            id: 1,
            text: "Temos trabalhado com a Positivus desde o ano passado e temos visto um crescimento significativo em tráfego no website e leads. A equipe é profissional, responsiva, e realmente querem saber do sucesso do nosso negócio.",
            name: "John Smith",
            position: "Director de Marketing na ExCorp, Lda",
        },
        {
            id: 2,
            text: "Grata pelo profissionalismo deles, nossa empresa cresceu sua presença online significativamente. É uma alegria trabalhar com eles!",
            name: "Sarah Kim",
            position: "Directora de Marketing na XMedia",
        },
        {
            id: 3,
            text: "As soluções deles turbinaram nosso SEO e a performance das redes sociais. Recomendo!",
            name: "Emily Johnson",
            position: "CEO na AdBoost",
        },
        {
            id: 4,
            text: "Trabalhamos juntos por um ano e conseguimos alcançar objectivos e metas nunca antes vistas.",
            name: "Eric Worsten",
            position: "Design de Produtos na Castglow",
        },
        {
            id: 5,
            text: "Um crescimento exponencial. Trabalhar com a Positivus foi a melhor escolha que poderiamos ter feito para a nossa empresa.",
            name: "Slandio Soares",
            position: "CEO na Unitech, Lda",
        }
      ]

</script>

<style scoped>
swiper-container {
    width: 100%;
    height: 100%;
    padding-top: 2rem;
    padding-bottom: 2rem;
    width: auto !important;
}

swiper-slide {
    padding-bottom: 4rem;
}

.card {
  background-color: #191A23;
  height: 200px !important;
  position: relative;
  border-radius: 2rem;
  border: 1px solid #B9FF66;
}

.swiper-button-custom-prev,
.swiper-button-custom-next {
  color: #ffffff;
  padding: 10px;
  position: absolute;
  z-index: 10;
  cursor: pointer;
  font-size: 24px;
}

.swiper-button-custom-prev {
  bottom: 4.25rem;
  left: 33%;
}

.swiper-button-custom-next {
  bottom: 4.25rem;
  right: 33%;
}

/* BREAKPOINTS */
@media (max-width: 640px) {
  .swiper-button-custom-prev {
    left: 20%;
  }

  .swiper-button-custom-next {
    right: 20%;
  }
}

@media (max-width: 576px) {
  .swiper-button-custom-prev {
    left: 10%;
  }

  .swiper-button-custom-next {
    right: 10%;
  }
}

</style>
