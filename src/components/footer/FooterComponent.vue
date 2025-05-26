<template>
  <footer class="container-lg p-0">
    <div class="content-box">
        <div class="d-flex flex-column flex-sm-row justify-content-between align-items-center flex-wrap">
            <a href="/" class="mb-4 mb-sm-0">
                <img src="/img/logowhite.png" alt="">
            </a>
            <ul class="navbar-nav align-items-center  flex-column flex-sm-row">
                <li class="nav-item">
                    <a class="nav-link me-0 me-sm-3" aria-current="page" href="#">Sobre</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-0 me-sm-3" href="#">Serviços</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-0 me-sm-3" href="#">Casos de uso</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link me-0 me-sm-3" href="#">Preços</a>
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
        <div class="row my-5">
            <div class="col-12 col-lg-6 d-flex flex-column justify-content-center align-items-sm-start align-items-center">
                <h5 class="footer_title rounded-2 p-1 mb-4">Fale conosco:</h5>
                <span class="email_footer text-white mb-3">Email: info@positivus</span>
                <span class="phone_footer text-white mb-3">Telefone: +244 222 555 565</span>
                <span class="address_footer text-white mb-sm-0 mb-5">Endereço: Avenida Luther King, 123</span>
            </div>
            <div class="col-12 col-lg-6">
                <div class="news_letter">
                    <form class="form h-100 d-flex flex-column flex-sm-row justify-content-center align-items-center ps-sm-5 pe-sm-5 p-3">
                        <input type="email" name="email" id="email" placeholder="Email">
                        <button class="btn btn_newsletter">Subscrever</button>
                    </form>
                </div>
            </div>
        </div>
        <div class="rights_reserved text-white pt-5 d-flex flex-column flex-sm-row align-items-center align-items-sm-center justify-content-center justify-content-sm-start">
            <span class="me-0 me-sm-3">© 2023 Positivus. Todos os direitos reservados</span>
            <span><a href="#" class="nav-link">Privacidade</a></span>
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

.footer_title {
    background-color: #B9FF66;
}

.news_letter {
    background-color: #292A32;
    height: 100%;
    border-radius: 1rem;
}

.form {
    gap: 1rem;
}

#email {
    width: 50%;
    border: 1px solid #ffffff;
    outline: none;
    border-radius: .8rem;
    padding: 1rem;
    background: transparent;

}

#email::placeholder {
    color: #ffffff;
}
.btn_newsletter {
    width: 50%;
    padding: 1rem;
    background-color: #B9FF66;
    border-radius: .8rem !important;

}

.rights_reserved {
    border-top: 1px solid #ffffff;
}
@media (max-width: 992px) {
    .content-box {
        border-radius: 0;
        padding: 3rem;
    }
}


@media (max-width: 576px) {
    .content-box {
        padding: 3rem 1rem 1rem 1rem;
    }

    #email {
        width: 100%;
    }

    .btn_newsletter {
        width: 100%;
    }
}


</style>
