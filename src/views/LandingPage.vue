<script setup lang="ts">
import Header from "../components/Header.vue";
import Hero from "../components/Hero.vue";
import TopThree from "../components/TopThree.vue";
import Information from "../components/Information.vue";
import Leistungen from "../components/Leistungen.vue";
</script>

<template>
  <div>
    <Header class="mb-12" />
    <Hero />

    <div class="my-12 grid gap-10 bg-[#E5F5F7] px-5 py-16 md:px-20 lg:px-24">
      <TopThree />
      <Information />
    </div>

    <Leistungen class="mb-12 px-5" />
  </div>
</template>
