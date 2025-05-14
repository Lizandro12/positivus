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

</script>