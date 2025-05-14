<template>
    <div class="container py-4">
        <swiper-container
        :pagination="false"
        :loop="true"
        :autoplay-delay="2500"
        :autoplay-disable-on-interaction="false"
        :breakpoints= "{
            576: {
              slidesPerView: 1,
              spaceBetween: 5
              },
            640: {
              slidesPerView: 2,
              spaceBetween: 8
            },
            768: {
              slidesPerView: 3,
              spaceBetween: 8
            },
            992: {
              slidesPerView: 4,
              spaceBetween: 20
            },
            1200: {
              slidesPerView: 5,
              spaceBetween: 20
            }
            }">
            <swiper-slide v-for="(item, index) in 6" :key="index"><img class="partner-img" :src="`/img/partner-${index + 1}.png`" alt=""></swiper-slide>
        </swiper-container>
    </div>
</template>

<style scoped>

swiper-container {
    width: 100%;
  }

swiper-slide {
    text-align: center;
    font-size: 18px;
    background: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
}

swiper-slide img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

</style>