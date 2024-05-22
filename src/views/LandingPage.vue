<script setup lang="ts">
import Header from "../components/Header.vue";
import Hero from "../components/Hero.vue";
import TopThree from "../components/TopThree.vue";
import Information from "../components/Information.vue";
</script>

<template>
  <div>
    <Header />
    <Hero />

    <div class="my-12 grid gap-10 bg-[#E5F5F7] px-5 py-16 md:px-20 lg:px-24">
      <TopThree />
      <Information />
    </div>
  </div>
</template>
