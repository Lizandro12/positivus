<template>
    <nav class="navbar navbar-expand-lg py-4">
        <div class="container-fluid">
            <a class="navbar-brand" href="#" style="width: 180px;">
                <img class="img-fluid w-100" src="/img/logo.png" alt="">
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
                <div class="offcanvas-header">
                    <a href="#" style="width: 120px;">
                        <img class="img-fluid w-100" src="/img/logo.png" alt="">
                    </a>
                    <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                </div>
                <div class="offcanvas-body">
                    <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Sobre</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Serviços</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Casos de uso</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Preços</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Blog</a>
                        </li>
                    </ul>
                    <button-outline-component :_str="message"/>

                </div>
            </div>
        </div>
    </nav>
</template>

<script setup>
import ButtonOutlineComponent from '../utils/ButtonOutlineComponent.vue';

const message = "Pedir orçamento"



</script>