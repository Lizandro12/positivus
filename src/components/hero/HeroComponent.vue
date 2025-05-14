<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-md-6">
                <h1 class="hero_title my-4">Navegando no cenário digital para o sucesso</h1>
                <p class="hero_paragraph">Nossa agência de marketing digital ajuda empresas a crescer e ter sucesso online por meio de uma variedade de serviços, incluindo SEO, PPC, marketing de mídia social e criação de conteúdo.</p>
                <div class="mt-4">
                    <button-component :_str="message"/>
                </div>
            </div>
            <div class="col-12 col-md-6">
                <img class="w-100 mt-4" src="/img/hero-img.png" alt="">
            </div>
        </div>

    </div>
</template>

<script setup>
import ButtonComponent from '../utils/ButtonComponent.vue';

const message = "Agendar consultoria"


</script>

<style>

</style>