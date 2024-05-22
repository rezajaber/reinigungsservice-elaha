<script setup lang="ts">
import Header from "../components/Header.vue";
import Hero from "../components/Hero.vue";
import TopThree from "../components/TopThree.vue";
import Information from "../components/Information.vue";
import Leistungen from "../components/Leistungen.vue";
import Vorteile from "../components/Vorteile.vue";
import Engagement from "../components/Engagement.vue";
import Einsatzgebiete from "../components/Einsatzgebiete.vue";
import ContactUs from "../components/ContactUs.vue";
import Footer from "../components/Footer.vue";
import Testimonials from "../components/Testimonials.vue";
</script>

<template>
  <div>
    <Header class="fixed inset-x-0 top-0 z-10 bg-white" />
    <Hero class="mt-40" />

    <div class="my-16 grid gap-10 bg-primary px-5 py-16 md:px-20 lg:px-24">
      <TopThree />
      <Information />
    </div>

    <Leistungen class="mb-12 px-5 md:px-20 xl:px-0" />
    <Vorteile class="mb-12 px-5 md:px-20 xl:px-0" />
    <Testimonials />

    <Einsatzgebiete class="mb-12 px-5 md:px-20 xl:px-0" />
    <ContactUs class="bg-primary px-5 py-8 md:px-20 md:py-20 xl:px-0" />
    <Footer class="bg-popover-foreground py-12" />
  </div>
</template>
