<template>
    <div class="redesign rounded-5 container">
        <div class="row">
            <div class="col-12 col-lg-6 d-flex flex-column justify-content-center text-center text-lg-start">
                <h3 class="redesign_title">Vamos fazer as coisas acontecerem</h3>
                <p class="my-4 redesign_paragraph">Entre em contacro hoje para saber como os nossos serviços de marketing digital podem ajudar o seu negócio a crescer e ter sucesso online.</p>
                <button-component :_str="message"/>
            </div>
            <div class="col-12 col-lg-6 redesig_image_container d-none d-lg-inline position-relative">
                <div class="d-flex justify-content-center"> 
                    <img  class="redesign_image img-fluid position-absolute" src="/img/make-things.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import ButtonComponent from './ButtonComponent.vue';

const message = "Receber apresentação de graça"
</script>


<style scoped>

.btn-cta:hover{
    background-color: #B9FF66;
    color: #191A23 !important;
    box-shadow: 5px 5px 0px 0px #191A23;
}



</style>