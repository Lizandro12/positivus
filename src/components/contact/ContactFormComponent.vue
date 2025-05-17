<template>
    <div class="container mt-5 mb-5">
        <div class="d-flex flex-column flex-lg-row align-items-center pt-4 pb-5">
            <h2 class="title rounded me-0 me-sm-5">Contacto</h2>
            <p class="paragraph text-center text-lg-start">Conecte-se a nós: Vamos discutir suas necessidades de Marketing Digital.</p>
        </div>
        <div class="contact_form_container">
            <div class="row">
                <div class="col-12 col-lg-6 form_side">
                    <div class="mb-4 d-flex d-sm-block justify-content-between">
                        <label for="hi" class="me-4">
                            <input type="radio" name="hi" id="hi">
                            Diga Olá
                        </label>
                        <label for="cote">
                            <input type="radio" name="cote" id="cote">
                            Pedir quotação
                        </label>
                    </div>
                    <form>
                        <div class="mb-3">
                            <label for="name" class="form-label">
                                Nome *
                            </label>
                            <input type="text" class="form-control contact_input contact_input-name" placeholder="Nome">
                        </div>
                        <div class="mb-3">
                            <label for="email" class="form-label">
                                Email *
                            </label>
                            <input type="email" class="form-control contact_input contact_input-email" placeholder="Email">
                        </div>
                        <div class="mb-3">
                            <label for="message" class="form-label">
                                Mensagem *
                            </label>
                            <textarea name="message" id="message" cols="55" rows="7" class="form-control contact_input contact_input-textarea" placeholder="Mensagem"></textarea>
                        </div>
                        <div class="">
                            <button class="btn btn-form w-100">Enviar mensagem</button>
                        </div>
                    </form>
                </div>
                <div class="col-12 col-lg-6 d-none d-lg-flex justify-content-end align-items-center" >
                    <div class=" img_side" style="width: 295px; height: 515px;">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>