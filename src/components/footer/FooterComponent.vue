<template>
  <footer class="container-lg p-0">
    <div class="content-box">
        <div class="d-flex justify-content-between align-items-center flex-wrap">
            <a href="/">
                <img src="/img/logowhite.png" alt="">
            </a>
            <ul class="navbar-nav flex-row">
                <li class="nav-item">
                    <a class="nav-link me-3" aria-current="page" href="#">Sobre</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-3" href="#">Serviços</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-3" href="#">Casos de uso</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-3" href="#">Preços</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Blog</a>
                </li>
            </ul>
            <ul class="navbar-nav flex-row">
                <li class="nav-item">
                    <a class="nav-link me-3" aria-current="page" href="#">
                        <img src="/img/linkedind.png" alt="">
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-3" href="#">
                        <img src="/img/facebook.png" alt="">
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me" href="#">
                        <img src="/img/twiter.png" alt="">
                    </a>
                </li>
            </ul>
        </div>

    </div>
  </footer>
</template>

<script setup>


</script>

<style scoped>
.content-box {
    background-color: #191A23;
    border-radius: 2rem 2rem 0 0;
    padding: 3rem;
}

.nav-link {
    color: #ffffff !important;
    text-decoration: underline;
}

@media (max-width: 992px) {
.content-box {
    border-radius: 0;
    padding: 3rem;
}
}

</style>
