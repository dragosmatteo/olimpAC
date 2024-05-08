<script setup>
import About from "./components/AboutComponent.vue";
import Calendly from "./components/CalendlyComponent.vue";
import Footer from "./components/FooterComponent.vue";
import Header from "./components/HeaderComponent.vue";
import Hero from "./components/HeroComponent.vue";
import Testimonial from "./components/TestimonialComponent.vue";
</script>

<template>
  <div class="w-full h-auto bg-black pt-[35px] overflow-x-hidden">
    <div class="px-[35px] lg:px-[35px] xl:px-[0px]">
      <Header />
      <Hero />
      <About />
      <Calendly />
      <Testimonial />
    </div>
    <Footer />
  </div>
</template>
