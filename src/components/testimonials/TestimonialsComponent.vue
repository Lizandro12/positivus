<template>
  <div class="py-5 container testimonial">
    <swiper-container
      :modules="[Pagination]"
      :space-between="50"
      :navigation="true"
      :pagination="{
        el: '.custom-pagination',
        clickable: true,
        renderBullet: renderCustomBullet()
      }"
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
  </div>
</template>

<script setup>
import { Pagination } from 'swiper/modules';

const bullet_1 = "/img/pagination_1.png"
const bullet_2 = "/img/pagination_2.png"

const renderCustomBullet = (index, className)=> {
    return `
    <span class="${className}">
        <img src="${bullet_2}" alt="paginação">
    <span/>
    `;
}


const testimonials =  [
        {
            id: 1,
            text: "We have been working with Positivus for the past year and have seen a significant increase in website traffic and leads. The team is professional, responsive, and truly cares about the success of our business.",
            name: "John Smith",
            position: "Director de Marketing na ExCorp, Lda",
        },
        {
            id: 2,
            text: "Thanks to their expertise, our company has grown its online presence significantly. They're a joy to work with!",
            name: "Sarah Kim",
            position: "Marketing Director at XMedia",
        },
        {
            id: 3,
            text: "Their solutions boosted our SEO and social media performance. Highly recommended!",
            name: "Emily Johnson",
            position: "CEO at AdBoost",
        },
        {
            id: 4,
            text: "Their solutions boosted our SEO and social media performance. Highly recommended!",
            name: "Emily Johnson",
            position: "CEO at AdBoost",
        },
        {
            id: 5,
            text: "Their solutions boosted our SEO and social media performance. Highly recommended!",
            name: "Emily Johnson",
            position: "CEO at AdBoost",
        }
      ]

</script>

<style scoped>
swiper-container {
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

.custom-pagination {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-top: 1rem;
}

.swiper-pagination-bullet {
  width: 20px;
  height: 20px;
}

.swiper-pagination-bullet img {
  width: 100%;
  height: auto;
  transition: filter 0.3s ease;
}

/* Quando o bullet estiver ativo, troca para a imagem verde */
.swiper-pagination-bullet-active img {
  content: url('/img/bullet-green.png');
}
</style>
