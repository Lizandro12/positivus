<template>
    <div>
        <header class="container">
            <header-component/>
        </header>
        <main>
            <section>
                <hero-component/>
            </section>
            <section>
                <partner-component/>
            </section>
            <section>
                <services-component/>
            </section>
            <section>
                <make-things-happen-component/>
            </section>
            <section>
                <cases-studie-component/>
            </section>
            <section>
                <how-it-works-accordion-component/>
            </section>
            <section>
                <our-team-component/>
            </section>
            <section>
                <testimonials-component/>
            </section>
            <section>
                <contact-form-component/>
            </section>
            <footer-component/>
        </main>
    </div>
</template>

<script setup>
import HeaderComponent from './header/HeaderComponent.vue';
import HeroComponent from './hero/HeroComponent.vue';
import PartnerComponent from './hero/PartnerComponent.vue';
import ServicesComponent from './ourservices/ServicesComponent.vue';
import MakeThingsHappenComponent from './utils/MakeThingsHappenComponent.vue';
import CasesStudieComponent from './cases/CasesStudieComponent.vue';
import HowItWorksAccordionComponent from './accordion/HowItWorksAccordionComponent.vue'; 
import OurTeamComponent from './team/OurTeamComponent.vue';
import TestimonialsComponent from './testimonials/TestimonialsComponent.vue';
import ContactFormComponent from './contact/ContactFormComponent.vue'
import FooterComponent from './footer/FooterComponent.vue';

import Typebot from 'https://cdn.jsdelivr.net/npm/@typebot.io/js@0.3/dist/web.js'

Typebot.initBubble({
    typebot: "faq-092kq8q",
    theme: {
        button: { backgroundColor: "#1D1D1D" },
        chatWindow: { backgroundColor: "#fff" },
    },
});

</script>